---
title: 07-Flutter-详解
date: 2025-04-05 01:59:52
---

# Flutter 详解

Flutter 是 Google 推出的跨平台 UI 框架，可以同时为移动端、Web 和桌面开发应用。

## 核心特性

- 基于 Dart 语言
- 自绘高性能渲染引擎
- 丰富的组件和生态

## 基本用法

```dart
import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(home: Scaffold(body: Center(child: Text('Hello Flutter'))));
  }
}
```

## 适用场景

- 多平台统一 UI、高性能移动应用

---

## 关联文档

- [08-常用的技术框架.md](./08-常用的技术框架.md)