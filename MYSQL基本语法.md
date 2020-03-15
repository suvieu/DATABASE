通过命令行连接MYSQL 命令行切换到MYSQL安装目录中的bin目录下，输入mysql -hlocalhost -uroot -p password 其中-u后输入用户名，-p后输入密码

显示所有数据库：show databases;

创建数据库：CREATE DATABASE dbname;

使用数据库：USE dbname;

查看当前使用了哪个数据库：SELECT DATABASE();

删除数据库：DROP DATABASE dbname;

查看数据库中的表：SHOW TABLES;

查看表内所有内容：SELECT * FROM tbname;

创建新表：CREATE TABBLE table_name (column_name column_type); 比如 create table mtime(NAME varchar(250) PRIMARY KEY,LINK varchar(250),point int,YEAR varchar(250));

插入数据：INSERT INTO tbnames(column_name1,column_name2,column_name3...) values(value1,value2...)

查看表内数据类型：SHOW COLUMNS FROM tbname;

更改字段数据类型:alter table tbname modify column column_name new_data_type;


删除表内所有内容：DELETE FROM  tbname

按中文拼音排序：select * from musician_ordered order by convert(name using gbk) collate gbk_chinese_ci;

修改主键为其他列：1.alter table TABNAME drop primary key; 2‘alter table TABNAME add primary key(another_col,...);

