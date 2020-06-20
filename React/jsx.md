## jsx
  1. 每个组件最外层必须有```<div></div>```标签
  2. 想要包住组建，但是不希望展示出来可以用```<Fragment></Fragment>```代替

### 构造函数
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592676822174-1592676822176.png)
1. 每个组件类都以一个构造函数
2. 数据放在```this.state```中，如图所示



### jsx事件
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592676081395-1592676081418.png)

1. js表达式加```{}```
2. 绑定this，指定当前对象
3. 事件大写```onClick```
4. ```bind```

### arry.map()函数
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592676460030-1592676460060.png)

1. 每个arry里有个map函数
2. 必传参数为回调函数，每个元素放入到回调函数中执行，返回新书组
3. 回调函数参数：元素内容（必须），元素下表
4. ```<li>```标签必须有唯一key（项目中不要使用元素index，这里方便演示）


### ES6展开运算符

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592677114941-1592677114943.png)
1. 就是将数组拆开和后面的值合并成新数组




