---
title: Module-Federation-详解
date: 2025-04-05 04:30:00
permalink: 08-01-Module-Federation-详解.html
tags:
  - 前端工程化
  - Module Federation
categories:
  - 前端工程化
  - 08-常用的技术框架
  - Module-Federation-详解
---

# Module Federation 详解

Module Federation 是 Webpack 5 引入的一项革命性特性，允许多个独立构建的应用在运行时动态地共享模块，实现真正意义上的微前端架构。

## 核心特性

- 支持远程加载与暴露模块
- 运行时依赖共享
- 低耦合，高复用

## 典型用法

```js
// webpack.config.js (部分)
plugins: [
  new ModuleFederationPlugin({
    name: 'app1',
    remotes: { app2: 'app2@http://localhost:3002/remoteEntry.js' },
    exposes: { './Button': './src/Button' },
    shared: ['react', 'react-dom']
  })
]
```

## 适用场景

- 微前端架构
- 多团队协作开发
- 独立部署的前端子应用

---

## 关联文档

- [08-常用的技术框架.md](./08-常用的技术框架.md)