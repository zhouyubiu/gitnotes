## 概念

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/25/1593093846244-1593093846275.png)

1. 实现了HttpServlet中的service方法，tomcat会找到接口（该接口定义了service）的子类实现，运行其中的service方法


## 具体实现
1. 创建servlet类，继承HttpServlet类

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/25/1593094130996-1593094130998.png)

2.在web.xml文件中定义servlet以及mapping映射
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/25/1593094247592-1593094247594.png)


## servlet生命周期

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/25/1593097649798-1593097649803.png)

1. 请求到达服务端
2. tomcat加载将webxml文件加载到内存
3. 找到对应的servlet，根据mapping找到接口对应的实现子类
4. 执行service，doGet,doPost等方法 


## request常用方法


![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/26/1593154983714-1593154983753.png)


## servlet 处理流程

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/26/1593180952089-1593180952124.png)

## 请求转发
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/26/1593182432945-1593182432948.png)