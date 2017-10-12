## 开篇

安装create-react-app

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



 

