---
title: 08-11-Rspack-详解
date: 2025-04-05 04:10:00
permalink: 08-11-Rspack-详解.html
tags:
  - 前端工程化
  - 构建工具
categories:
  - 前端工程化
  - 技术框架
---

# Rspack 详解

Rspack 是由字节跳动推出的高性能 Web 构建工具，采用 Rust 语言实现，主打极致构建性能和现代前端工程体验。Rspack 致力于成为 webpack 的现代化替代，兼容 webpack 生态，并且在速度与资源利用率上有大幅提升。

## 核心特性

- 高性能（Rust 实现，天然多线程并行）
- 兼容 webpack 生态，便于迁移
- 现代特性支持（Tree Shaking、HMR、CSS Modules 等）
- 插件机制完善，支持 Rust/JS 插件

## 典型配置

```js
// rspack.config.js
module.exports = {
  entry: './src/index.js',
  output: { filename: 'bundle.js', path: __dirname + '/dist' },
  module: {
    rules: [
      { test: /\.js$/, loader: 'babel-loader' },
      { test: /\.css$/, use: ['style-loader', 'css-loader'] }
    ]
  }
}
```

## 适用场景

- 追求极致构建速度和体验的大型前端项目
- 需要兼容 webpack 配置和生态的团队

---

## 关联文档

- [08-常用的技术框架.md](./08-常用的技术框架.md)