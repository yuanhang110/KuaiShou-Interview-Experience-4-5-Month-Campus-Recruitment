#### 集合

4说一说知道哪些集合

List常用的实现类

ArrayList与LinkedList区别

5 ArrayList和LinkedList

6插入元素时间复杂度

7新建一个ArrayList会分配内存嘛

8 ArrayList扩容的时机

**9 ArrayList什么时候缩容**  

  10 LinkedList<Integer>插入int 

  11谁实现int装包的，是List吗 

  12 ArrayList线程安全吗，说说你知道的线程安全的List 

  13 Collections.同步方法和copyonwriteArrayList的异同点

ArrayList和LinkedList的区别

ArrayList扩容机制，上次看ArrayList源码还是去年9月份，，，真的忘了，只记得1.5倍扩容和grow方法的流程，其他的模模糊糊。我回答到当扩容1.5倍之后还不能满足大小，就直接将需要的大小设置为要扩容的大小。面试官可能将计就计的问了我add方法一次添加一个元素为什么会不满足条件呢，当时内心有点懵，所以也没回答出来，面试官又问如果让你去写这个代码，你觉得的该怎么写，只说思路就好。我就讲了一下自己的想法，这才结束了这个话题，害，健忘的我。

面试官在对话框里列出了ArrayList很多API，让我逐个分析他们的时间复杂度。

2.hashmap的复杂度 O(1)，有链表还得算链表，大于8变红黑树 

hahsmap的扩容。
答：就是新开一个2倍大小的空间，然后用头插法插入到新的位置；而1.8版本的话，是会用位运算求出节点的位置。

万年不变的集合开头，hashmap底层数据结构，什么时候转化为红黑树，put操作的流程，讲定位下标的时候说到了扰动，又问扰动的过程和好处（讲一半小哥哥网不稳定，掉线了，，，）    

hashmap线程安全吗？线程安全的方式有哪些？    

concurrenthashmap怎么样去保证线程安全的    

5.hashmap、hashtable、concurrenthashmap

讲讲hashmap

HashMap底层数据结构实现
红黑树能不能再变回链表
为什么在8个的时候转化为红黑树
HashMap是线程安全的吗
如果一个在读写操作，另一个在扩弄，会不会有问题

5：并发包、ConcurrentHashMap等

5.HashMap底层数据结构，以及put方法和resize方法 	

6.说一下ConcurrentHashMap底层数据结构，以及如何保证线程安全的 

讲讲java中的集合类，Comparable接口和Comparator接口