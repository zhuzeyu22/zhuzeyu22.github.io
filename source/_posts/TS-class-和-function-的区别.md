---
title: TS class 和 function 的区别
date: 2023-05-30 13:30:50
tags:
---

# 相同点

- class 和 function 都可以作为构造函数，通过 new 操作符来实例化。

---

# 不同点

## 1. class 构造函数必须使用 new 操作符

- 普通 function 构造函数把 window 作为 this 来创建实例
- 调用 class 构造函数时如果忘了使用 new 则会抛出错误

## 2. class 声明不可以提升

- function 构造函数声明存在提升，也就是定义构造函数的部分可以写在实例化对象的后面

  ```js
  const usr = new Person("Jack");
  console.log(usr); // Person { name: 'Jack' }

  function Person(name) {
    this.name = name;
  }
  ```

- class 声明不存在提升，声明类的部分不能写在实例化对象的后面

  ```js
  const usr = new Person("Jack");
  // ReferenceError: Cannot access 'Person' before initialization

  class Person {
    constructor(name) {
      this.name = name;
    }
  }
  ```

## 3. class 不可以用 call、apply、bind 改变执行上下文

Ref: [call、apply、bind 具体使用方式](https://lzxjack.top/post?title=call-apply-bind)
