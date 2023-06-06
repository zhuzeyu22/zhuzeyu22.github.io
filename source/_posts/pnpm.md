---
title: pnpm
date: 2023-05-31 10:35:25
tags:
---

# [依赖配置 npmrc](https://pnpm.io/zh/npmrc)

- 处理依赖不同版本的包时

  ```
  pnpm config set auto-install-peers true --location project
  ```

# [link](https://pnpm.io/zh/cli/link)

- 本地开发环境使用 pnpm link

  别名: ln

  使当前本地包可在系统范围内或其他位置访问。

  ```
  pnpm link <dir>
  pnpm link --global
  pnpm link --global <pkg>
  ```
