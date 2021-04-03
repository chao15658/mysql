# postgresql和mysql区别

时间类型

**mysql                                   postgres**

datetime                               timestamp ( timestamp without time zone )

自增列

serial                                     AUTO_INCREMENT

on update                             借助trigger



时间操作

减法    Date_Sub                      -

 加法   date_add                       +

格式化 date_format              to_char

随机数 Rand                           random



存储过程语法

WHILE do                                 while loop 

end WHILE ；                              end loop；



创建分区表

 create table xx(                               create table t1(

  id int)                                                         id int

partation by list(id) (                          ) partation by list(id );

partation p1 values in(2)                  create tt1 partation of t1 for values in(2);

partation p1 values in(3)                   create tt2 partation of t1 for values in(3);

);                                                        



update语句

update t1 b,t2 a                                 update t1 

set b.id=a.id                                        set id=a.id

where a.id=b.id;                                  from t1 b,t2 a

​                                                               where a.id=b.id;