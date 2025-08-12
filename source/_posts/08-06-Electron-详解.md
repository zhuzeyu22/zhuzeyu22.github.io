---
title: 08-06-Electron-详解
date: 2025-04-05 04:20:00
permalink: 08-06-Electron-详解.html
tags:
  - 前端工程化
  - 桌面应用
categories:
  - 前端工程化
  - 技术框架
---

# Electron 详解

Electron 是基于 Chromium 和 Node.js 的跨平台桌面应用开发框架。

## 核心特性

- 跨平台（Windows/Mac/Linux）
- 主进程 + 渲染进程架构
- 可集成系统原生能力

## 基本用法

```js
const { app, BrowserWindow } = require('electron')
app.on('ready', () => {
  new BrowserWindow({ width: 800, height: 600 }).loadURL('https://example.com')
})
```

## 适用场景

- 桌面客户端、开发工具、跨平台应用

---

## 关联文档

- [08-常用的技术框架.md](./08-常用的技术框架.md)