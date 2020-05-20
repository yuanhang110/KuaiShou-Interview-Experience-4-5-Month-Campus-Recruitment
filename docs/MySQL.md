#### 数据库

##### MySQL

MySql存储引擎都有什么

MyISAM的优点是什么？查询为什么这么快

6.**[MyISAM和InnoDB的区别](http://www.cnblogs.com/zhangchaoyang/articles/4214237.html)**

37 MySQL用的是什么引擎，索引是啥

Myisam与InnoDB的区别
如何理解事务，事务解决了什么问题
ACID
事务的隔离级别

5.事务的隔离级别和事务并发的问题

7.事务的ACID特性，然后说了下事务隔离级别以及数据库上的实现。删除一条不存在的数据会加锁吗（emmm，没试过）

脏读，不可重复读，幻读

InnoDB解决幻读了吗
如果第一次Select出来只有一条，第二次出来是两条，这是幻读吗

第一次查询张三这个人系统没有，尝试插入张三，提示主键重复，是不是幻读


聚集索引
联合索引底层是什么结构什么样子的
讨论例子能不能命中索引

写SQL的注意事项 

写个sql：课程名中包含‘计算机’的课程 且 成绩小于60分学生的 学号、姓名

```mysql
SELECT stu.id, stu.name FROM stu, stu_score WHERE stu_score.coursename = '计算机'
AND stu_score.score <60 AND stu.id = stu_score.stuid
```

数据库中JOIN是怎么实现的，IN呢

4.mysql索引

4.mysql的索引，分页查找，如果要查找很靠后的页面如何，比如100万之后查10条怎么优化（）

6.数据库索引、非聚簇索引和聚簇索引

讲下MySQL的聚簇索引

聚簇索引哪个引擎在用？只有InnoDB吗？

InnoDB索引采取什么数据结构

说说聚集索引和非聚集索引，mysql的4种事务隔离级别，InnoDB在Repeatable_Read下为什么不会幻读，索引为什么用B+树，B+树和B树的区别

7.数据库索引底层数据结构是什么样的

6.next_lock,快照读和当前读，MVCC

6.数据库问题，表结构是t <id, a, b, c>，sql语句是select * from t where a= , b= , c= 问这个语句执行的效率，我当时直接说会很慢，可以建立联合索引，然后就开始了最左匹配原则的各种情况。最后一个问题是如果查询条件固定，联合索引的顺序怎么样安排比较好，之前没考虑过，只能当场思考，回答的是区分度较高的排在前面，让搜索的范围尽早缩小。可能解释不太明白，面试官出了具体的场景问我，才作罢。

动态SQL  

order by在数据库innodb的实现过程没答出来  

limit会对前面的数据进行IO吗  

数据量大limit的解决方案  

数据库一定会走索引吗回答了最左匹配原则和索引没及时更新数据位置，没答到他想要的点，他想问的是where语句中出现了!=，会走索引吗  

K>某个值，索引会失效吗？MySQL会判断一下全盘扫描的成本和走索引的成本

Elasticsearch 是一个分布式、可扩展、实时的搜索与数据分析引擎

es有哪两种交互方式？

es底层数据结构（不知道）lucene