# AQS
- 内部维护了一个 ==volatile int state== (具体含义看子类如何实现)
- CLH队列：双向链表，每个节点存放一个线程,(CAS的方式维护头尾)

<img src="https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/04/27/1588000559014-1588000559019.png" weight=800 height=400     />


- acquierd
