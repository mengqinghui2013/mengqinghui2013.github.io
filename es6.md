## 1. ECMASCRIPT 和 JAVASCRIPT的关系

ECMAScript 和 JavaScript 的关系是，前者是后者的规格，后者是前者的一种实现（另外的 ECMAScript 方言还有 Jscript 和 ActionScript）

## 2. 语法提案的批准流程

Stage 0 - Strawman（展示阶段）

* Stage 1 - Proposal（征求意见阶段）
* Stage 2 - Draft（草案阶段）
* Stage 3 - Candidate（候选人阶段）
* Stage 4 - Finished（定案阶段）

一个提案只要能进入 Stage 2，就差不多肯定会包括在以后的正式标准里面。ECMAScript 当前的所有提案，可以在 TC39 的官方网站

[Github.com/tc39/ecma262](https://github.com/tc39/ecma262) 查看。



## 3. let/const/var

1.   块级作用域 
2.   变量提升
3.   允许重复定义吗
4. `const`实际上保证的，并不是变量的值不得改动，而是变量指向的那个内存地址不得改动 



var a = \[\];

for \(let i = 0; i &lt; 10; i++\) {

  a\[i\] = function \(\) {

    console.log\(i\);

  };

}

a\[6\]\(\); 



## 4. 变量的解构赋值

ES6 允许按照一定模式，从数组和对象中提取值，对变量进行赋值，这被称为解构（Destructuring）

用法

1. 数组

let \[a, b, c\] = \[1, 2, 3\];

let \[ , , third\] = \["foo", "bar", "baz"\];

third // "baz"

  2. 对象

   let { bar, foo } = { foo: "aaa", bar: "bbb" };



   **变量名和key不匹配怎么办？**

   let { foo: baz } = { foo: 'aaa', bar: 'bbb' };

baz // "aaa"

  3. 默认值

      let \[x, y = 'b'\] = \['a', 2\]; // x='a', y='b'

   **   什么时候使用默认值？**



  4. null/undefined 处理

let { prop: x } = undefined; // TypeError

let { prop: y } = null; // TypeError



## 5. 函数拓展

1. 函数默认值
2. rest 参数
   1. ES6 引入 rest 参数（形式为`...变量名`），用于获取函数的多余参数，这样就不需要使用`arguments`对象了。rest 参数搭配的变量是一个数组

   2. rest 参数之后不能再有其他参数（即只能是最后一个参数
3. name 属性  匿名函数ES5 返回''

   1. bind返回的函数，name属性值会加上bound前缀。

   2. bind 后的函数和原来是一样的嘛？

   3. 

4. 箭头函数

   1. **函数体内的this对象，就是定义时所在的对象，而不是使用时所在的对象**

   2. 不可以当作构造函数，也就是说，不可以使用new命令，否则会抛出一个错误

   3. 不可以使用arguments对象，该对象在函数体内不存在。如果要用，可以用 rest 参数代替

   4. 不可以使用yield命令，因此箭头函数不能用作 Generator 函数

## 6. 扩展运算符 ...

console.log\(1, ...\[2, 3, 4\], 5\)

 对象使用场景

1.   解构 let { x, y, ...z } = { x: 1, y: 2, a: 3, b: 4 };
2.   拷贝赋值 let z = { a: 3, b: 4 };
   let n = { ...z };
   n // { a: 3, b: 4 }











