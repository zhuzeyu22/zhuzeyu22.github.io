---
title: webpack-plugins
date: 2023-05-25 10:16:19
tags:
---

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

---

# 循环依赖分析

- CircularDependencyPlugin

  usage

  https://www.npmjs.com/package/circular-dependency-plugin

---

# 清空 output 目录中内容

- clean-webpack-plugin

  usage

  https://www.npmjs.com/package/clean-webpack-plugin

---

# 复制源码文件

- copy-webpack-plugin

  usage

  https://www.npmjs.com/package/copy-webpack-plugin

---

# 内容安全 CSP （Content Security Policy）

- CSP 定义

  https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy

- csp-html-webpack-plugin

  usage

  https://www.npmjs.com/package/csp-html-webpack-plugin

---

# css 优化插件

- css-minimizer-webpack-plugin

  usage

  https://www.npmjs.com/package/css-minimizer-webpack-plugin

---

# 编译和优化 插件

比 babel-loader/ts-loader 更快

比 Terser 更小

- esbuild-loader

  usage

  https://www.npmjs.com/package/esbuild-loader

---

# 字体图标插件

- fantasticon

  usage

  https://www.npmjs.com/package/fantasticon

# 使用独立进程进行 TS 类型检查

- fork-ts-checker-webpack-plugin

  usage

  https://www.npmjs.com/package/fork-ts-checker-webpack-plugin

---

# 将 bundle 打包成 H5 文件

- html-webpack-plugin

  uasage

  https://www.npmjs.com/package/html-webpack-plugin

---

# 图像压缩插件

- image-minimizer-webpack-plugin

  usage

  https://www.npmjs.com/package/image-minimizer-webpack-plugin

# css 压缩插件

- mini-css-extract-plugin

  usage

  https://www.npmjs.com/package/mini-css-extract-plugin
