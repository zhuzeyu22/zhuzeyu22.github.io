---
title: decorator
date: 2023-05-30 10:16:23
tags:
---

# TS decorator

- Ref: https://www.tslang.cn/docs/handbook/decorators.html

- 虽然是实验特性，鉴于 python、 java、lua 里面都有类似的东西，以后必然 TS 会支持。

- 装饰器是一种特殊类型的声明，它能够被附加到类声明，方法， 访问符，属性或参数上。

---

## 装饰器工厂

```ts
function color(value: string) {
  // 这是一个装饰器工厂
  return function (target) {
    //  这是装饰器
    // do something with "target" and "value"...
  };
}
```

---

## 装饰器组合

- 书写在同一行上：

```
@f @g x

```

- 书写在多行上：

```
@f
@g
x
```

```ts
function f() {
  console.log("f(): evaluated");
  return function (
    target,
    propertyKey: string,
    descriptor: PropertyDescriptor
  ) {
    console.log("f(): called");
  };
}

function g() {
  console.log("g(): evaluated");
  return function (
    target,
    propertyKey: string,
    descriptor: PropertyDescriptor
  ) {
    console.log("g(): called");
  };
}

class C {
  @f()
  @g()
  method() {}
}
```

结果如下：

```
f(): evaluated
g(): evaluated
g(): called
f(): called
```

---

## 装饰器求值

1. 参数装饰器，然后依次是方法装饰器，访问符装饰器，或属性装饰器应用到每个实例成员。
2. 参数装饰器，然后依次是方法装饰器，访问符装饰器，或属性装饰器应用到每个静态成员。
3. 参数装饰器应用到构造函数。
4. 类装饰器应用到类。

---

## 类装饰器

// todo

---

## 方法装饰器

// todo

---

## 访问器装饰器

// todo

---

## 属性装饰器

// todo

---

## 参数装饰器

// todo
