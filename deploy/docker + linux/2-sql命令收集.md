# SQL语句替换规则

```java
// 自主命名
【】

// 可选项
《》

// 赋值操作
( 变量 ) = " 值 "
```



# 数据库操作

```mysql
# 创建数据库:
( A ) = "if not exists"             // if ( 数据库不存在 ) 执行创建库
( B ) = "default charset 【字符集】"  // 指定编码格式
( C ) = "collate 【排序规则】"		// 指定排序规则
create database 《 A 》 `【库名】` 《 B 》 《 C 》;

# 删除数据库
( A ) = "if exists"  // if ( 数据库存在 ) 执行删除库
drop database 《 A 》 `【库名】`;

# 进入数据库
use `【库名】`;
```



# 表操作

```mysql
# 创建表
CREATE DATABASE `【表名】`;

# if (表存在) 删除表
DROP DATABASE 《 IF EXISTS  》`【表名】`;

```

