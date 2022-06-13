## Hive数据类型

###  基本数据类型

| 数据类型  | Java    | 长度         |
| --------- | ------- | ------------ |
| TINYINT   | byte    | 1 byte       |
| SMALINT   | short   | 2 byte       |
| INT       | int     | 4 byte       |
| BIGINT    | long    | 8 byte       |
| BOOLEAN   | boolean |              |
| FLOAT     | float   | 单精度浮点数 |
| DOUBLE    | double  | 双精度读点书 |
| STRING    | string  | 字符串       |
| TIMESTAMP |         |              |
| BINARY    |         |              |



### 集合数据类型

| 数据类型 | 描述                                                         | 实例             |
| -------- | ------------------------------------------------------------ | ---------------- |
| STRUCT   | 和 c 语言中的 struct 类似，都可以通过“点”符号访 问元素内容。例如，如果某个列的数据类型是 STRUCT{first STRING, last STRING},那么第 1 个元素可以通过字段.first 来 引用。 |                  |
| MAP      | MAP 是一组键-值对元组集合，使用数组表示法可以 访问数据。例如，如果某个列的数据类型是 MAP，其中键值对是’first’->’John’和’last’->’Doe’，那么可以通过字段名[‘last’]获取最后一个元素 | map<string, int> |
| ARRAY    | 数组是一组具有相同类型和名称的变量的集合。这些 变量称为数组的元素，每个数组元素都有一个编号，编号从 零开始。例如，数组值为[‘John’, ‘Doe’]，那么第 2 个元素可以通过数组名[1]进行引用。 | array\<string\>  |

Hive 有三种复杂数据类型 ARRAY、MAP 和 STRUCT。ARRAY 和 MAP 与 Java 中的 Array 和 Map 类似，而 STRUCT 与 C 语言中的 Struct 类似，它封装了一个命名字段集合，复杂数据 类型允许任意层次的嵌套。



### 类型转换 cast

例如 CAST('1' AS INT)将把字符串'1'  转换成整数 1；

如果强制类型转换失败，如执行 CAST('X' AS INT)，表达式返回空值 NULL。



## DDL

### 创建库

```sql
CREATE DATABASE [IF NOT EXISTS] database_name [COMMENT database_comment]
[LOCATION hdfs_path]
[WITH DBPROPERTIES (property_name=property_value, ...)];
```



### 切换数据库

```sql
USE database_name;
```



### 删除数据库

删不了非空数据库， **可以采用 cascade 命令，强制删除**

```sql
DROP IF EXISTS database_name
```



### 创建表

```sql
CREATE [EXTERNAL] TABLE [IF NOT EXISTS] table_name
[(col_name data_type [COMMENT col_comment], ...)] 
[COMMENT table_comment]
[PARTITIONED BY (col_name data_type [COMMENT col_comment], ...)] 
[CLUSTERED BY (col_name, col_name, ...)
[SORTED BY (col_name [ASC|DESC], ...)] INTO num_buckets BUCKETS] 
[ROW FORMAT row_format]
[STORED AS file_format] [LOCATION hdfs_path]
[TBLPROPERTIES (property_name=property_value, ...)] 
[AS select_statement]
```



### 重命名表

```sql
ALTER TABLE table_name RENAME TO new_table_name;
```



### 增加/修改/替换列信息

```sql
ALTER TABLE table_name CHANGE [COLUMN] col_old_name col_new_name column_type 
[COMMENT col_comment] [FIRST|AFTER column_name]
```



### 删除表

```sql
DROP TABLE IF EXISTS table_name;
```



## DML

### 插入数据insert

insert into：以追加数据的方式插入到表或分区，原有数据不会删除
insert overwrite：会覆盖表中已存在的数据



### as select 

```sql
create table if not exists student3 
as select id, name from student;
```



### sort by 每个reducer内部排序

 

### Distribute By 分区

Distribute By： 在有些情况下，我们需要控制某个特定行应该到哪个 reducer，通常是为 了进行后续的聚集操作。distribute by  子句可以做这件事。distribute by结合 sort by 使用。
对于 distribute by 进行测试，一定要分配多 reduce 进行处理，否则无法看到 distribute by 的效果。

+ distribute by 的分区规则是根据分区字段的 hash 码与 reduce 的个数进行模除后， 余数相同的分到一个
+ Hive 要求 DISTRIBUTE BY 语句要写在 SORT BY 语句之前。



### Cluster By

+ 当 distribute by 和 sorts by 字段相同时，可以使用 cluster by 方式。

+ cluster by 除了具有 distribute by 的功能外还兼具 sort by 的功能。但是排序只能是升序 排序，不能指定排序规则为 ASC 或者 DESC。



## 分区表

分区表实际上就是对应一个 HDFS 文件系统上的独立的文件夹，该文件夹下是该分区所 有的数据文件。Hive 中的分区就是分目录，把一个大的数据集根据业务需要分割成小的数据 集。在查询时通过 WHERE 子句中的表达式选择查询所需要的指定的分区，这样的查询效率 会提高很多



### 查看分区

```sql
desc formatted dept_partition;
```



### 二级分区

```sql
create table 
dept_partition2( deptno int, dname string, loc string
)
partitioned by (day string, hour string)

```



### 根据select字段名insert进不同分区

```sql
insert into table dept_partition_dy partition(loc) 
select deptno, dname, loc from dept;
```





## 常用函数

###  NVL(类似isnull)

```sql
nvl(T value, T default_value)

# Returns default value if value is null else returns value
```



### CONCAT(拼接字符)

```sql
concat(string|binary A, string|binary B...)


#Returns the string or bytes resulting from concatenating the strings or bytes passed in as parameters in order. 
#For example, concat('foo', 'bar') results in 'foobar'. Note that this function can take any number of input strings.

```



### CONCAT_WS(拼接字符)

```sql
concat_ws(string SEP, string A, string B...)
```



### EXPLODE(Array 或者 Map 结构拆分成多行)

```sql
explode(ARRAY<T> a)
#Explodes an array to multiple rows. Returns a row-set with a single column (col), one row for each element from the array.

explode(MAP<Tkey,Tvalue> m)
#Explodes a map to multiple rows. Returns a row-set with a two columns (key,value) , one row for each key-value pair from the input map. 

LATERAL VIEW
# 用法：LATERAL VIEW udtf(expression) tableAlias AS columnAlias

```

```sql
# array
SELECT tf.*
FROM (
    SELECT 0
) t
    LATERAL VIEW explode(array('A', 'B', 'C')) tf AS col;

# map
SELECT tf.*
FROM (
    SELECT 0
) t
    LATERAL VIEW explode(map('A', 10, 'B', 20, 'C', 30)) tf AS key, value;

# 与split一起用
SELECT
	movie, category_name
FROM
	movie_info lateral VIEW explode(split(category,",")) movie_info_tmp AS category_name;

```









