# 特点
- 函数式编程
- 参数类型自动推断
- 代码量少，简洁
- 本质上就是：定义接口，在调用的时候以 ==“()->{}”== 方式实现方法体

## 函数式接口
- 只有一个抽象方法的接口
- 加注解 ==@FunctionalInterface== 来限制

## 语法
- ==()==:写函数参数
- =={}==:代码块,只有一行代码时可以省略
 
# 函数式接口使用举例
```java
        Function<String,Integer> f1 = (str)->str.length();
        System.out.println(f1.apply("123"));
```

### 自定义接口
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/04/19/1587274423731-1587274423756.png)


### 可调用基本的静态函数方法

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/04/19/1587275778349-1587275778351.png)

实际上就是吧exec()方法放到了get方法中执行，仅此而已


#  方法引用

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/04/07/1586237802629-1586237802639.png)
 




