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
