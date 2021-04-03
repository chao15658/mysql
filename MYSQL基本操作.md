1、连接数据库

mysql  -uroot -p123456



2、连接具体的数据库

use +dbname



3、查看数据库列表

 show databases;



4.查看表列表

show tables;



5.查看模式列表

 show schemas;



6.查看用户列表

 `select user,host from mysql.user;`  



7、查看数据目录

 show global variables like "%datadir%"



8.查看安装目录

show global variables like "%basedir%";



9.查看配置信息

show global variables ;

