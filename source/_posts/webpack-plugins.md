---
title: webpack-plugins
date: 2023-05-25 10:16:19
tags:
---

# 代码分析插件

- BundleAnalyzerPlugin

  ```
  # linux
  webpack --profile --json > stats.json

  # windows
  webpack --profile --json | Out-file 'stats.json' -Encoding OEM

  # cli
  webpack-bundle-analyzer bundle/output/path/stats.json
  ```

# 循环依赖分析

- CircularDependencyPlugin

  usage

  https://www.npmjs.com/package/circular-dependency-plugin

# 清空 output 目录中内容

- clean-webpack-plugin

  usage

  https://www.npmjs.com/package/clean-webpack-plugin

# 复制源码文件

- copy-webpack-plugin

  usage

  https://www.npmjs.com/package/copy-webpack-plugin

# 内容安全 CSP （Content Security Policy）

- CSP 定义

  https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy

- csp-html-webpack-plugin

  usage

  https://www.npmjs.com/package/csp-html-webpack-plugin
