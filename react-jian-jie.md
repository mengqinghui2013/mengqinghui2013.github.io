## 开篇

安装create-react-app



## 要求

1. 课堂会有很多提问，大家尽量注意听讲
2. 知识点讲的比较细

## 

## 1. JSX 简介

1. jsx 属性 
2. jsx 防止xss漏洞
3. _dangerouslySetInnerHTML_

4. 属性含有转义字符怎么办

## 2. React 组件和props

1. React组件有几种生成方式
   1. function 形式
   2. class
2. 条件渲染有几种方式
   1. function if/else
   2. 变量赋值
   3. inline 形式 ， 比如 {condition && component}, 或者 ? : 操作
3. props / props.children
   1. pure function
   2. 属性不可修改
4. 如何挂载到dom元素上 ReactDOM.render\(\)

## 3. state 和 生命周期函数

1. setState 是 异步的吗？ this.state.a 的访问情况

2. didMount和unmount的作用

3. shouldUpdate的作用，如果shouldUpdate 返回了false，子组件的render还触发吗？哪些函数不再执行了？willUpdate和didUpdate，render 都不在触发了

4. setState触发后发生了什么？

5. ## 4. refs 和 dom元素

## 5. 事件

1.如何阻止默认行为？ return false 可以吗？

2.SyntheticEvent 是什么东西？

1. event 可以放到异步里面吗？  比如 setTimeout\(\(\) =&gt; {console.log\(event\)}, 1\)

## 6. JSX和HTML有什么区别？

1. 属性

2. 事件

3. 空格



