## jsx
  1. 每个组件最外层必须有```<div></div>```标签
  2. 想要包住组建，但是不希望展示出来可以用```<Fragment></Fragment>```代替

### 构造函数
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592676822174-1592676822176.png)
1. 每个组件类都以一个构造函数
2. 数据放在```this.state```中，如图所示



### jsx事件（bind）
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592676081395-1592676081418.png)

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592678900889-1592678900893.png)
1. js表达式加```{}```
2. 绑定this，指定当前对象
3. 事件大写```onClick```
4. ```bind```：第一个参数把当前对象绑定到时间函数内部，还可以传递参数到时间函数中

### arry.map()函数
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592676460030-1592676460060.png)

1. 每个arry里有个map函数
2. 必传参数为回调函数，每个元素放入到回调函数中执行，返回新书组
3. 回调函数参数：元素内容（必须），元素下表
4. ```<li>```标签必须有唯一key（项目中不要使用元素index，这里方便演示）


### ES6展开运算符

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592677114941-1592677114943.png)
1. 就是将数组拆开和后面的值合并成新数组

### 修改state中的数据

![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592679081970-1592679081973.png)

1. 凡事要操作```this.state```中的数据，首先拷贝一份，再执行操作（与react性能优化相关）
2. 操作完后统一在，```this.setState()```中赋值
3. 拷贝数组副本格式见上图list，可用展开符

### 去除html标签自动转义
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592680978726-1592680978730.png)
1. 使用标签中的```dangerouslySetInnerHTML```属性即可

### 输入框和label绑定
![title](https://raw.githubusercontent.com/zhouyubiu/gitnotes_images/master/gitnote/2020/06/21/1592681081135-1592681081137.png)
1. 点击标签，输入框获得光标，注意react中用htmlFor









