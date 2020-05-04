# AQS

- 内部维护了一个 ==volatile int state== (具体含义看子类如何实现)
- CLH队列：双向链表，每个节点存放一个线程,(CAS的方式维护头尾)

<img src="https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/04/27/1588000559014-1588000559019.png" weight=800 height=400     />

- varHandle的使用
jdk1.9以后
指向某个对象的引用，可以给普通的成员对象提供cas，原子相关的操作
可以理解为直接操作二进制码（效率优于反射）

<img src="https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/05/03/1588509410311-1588509410315.png" weight=800 height=400 />


# ThreadLocal
声明式事务中有使用
程序中两个线程，第一个线程改了对象中的属性的时候，第二个线程获取不到
原因是ThreadLocal的set把值存放在了当前线程的map（<ThreadLocal，Value>如图）里面仅对本线程可见，其他线程无法访问

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/05/04/1588524015792-1588524015795.png)



<img src="https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/05/04/1588523707398-1588523707404.png" weight=800 height=400 />


# 引用
强引用（普通Java对象引用）--------引用存在就不会回收

软引用（缓存）--------内存不够用才回收


弱引用（容器）-------------只要有垃圾回收就被会被回收

tl是ThreadLocal对象引用，是个抢强引用，key是个弱引用，tl消失时，key就会被回收变成null，但是value是个强引用，会一直在，所以ThreadLocal对象用完需要回收，否则造成内存泄漏。
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/05/04/1588526189791-1588526189812.png)

虚引用（回收收堆外内存）-----只要有垃圾回收就被会被回收，虚引用无法取到引用的值，被回收的时候会往队列（QUEUE）中丢一个值通知到该引用被回收，我们可以监测这个队列，当收到消息时，进行对外内存的回收。










