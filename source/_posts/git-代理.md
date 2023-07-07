---
title: git 代理
date: 2023-07-07 10:26:41
tags:
---

#使用socks5代理（推荐）（不可用）
git config --global http.https://github.com.proxy socks5://127.0.0.1:33210
#使用http代理（不推荐）(可用)
git config --global http.https://github.com.proxy http://127.0.0.1:33210

git config --global http.proxy http://127.0.0.1:33210

git config --global https.proxy https://127.0.0.1:33210

git config --global --unset http.proxy

git config --global --unset https.proxy

git config --global --unset http.proxy

git config --global --unset https.proxy


git config --global --unset http.https://github.com.proxy