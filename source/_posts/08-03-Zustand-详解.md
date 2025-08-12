---
title: 08-03-Zustand-详解
date: 2025-08-12 02:32:15
tags:
categories:
---

# Zustand 详解

Zustand 是一款轻量级、无依赖的 React 状态管理库，主打简洁和极致的开发体验。

## 核心特性

- 轻量、无依赖、Hooks API
- 支持中间件、可组合 store
- 性能优秀、易于维护

## 基本用法

```js
import create from 'zustand'
const useStore = create(set => ({
  count: 0,
  increment: () => set(state => ({ count: state.count + 1 }))
}))
```

## 适用场景

- 追求极致简单、轻量的 React 状态管理

---

## 关联文档

- [08-常用的技术框架.md](./08-常用的技术框架.md)