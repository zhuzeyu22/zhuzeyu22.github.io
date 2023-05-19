---
title: docker
date: 2023-05-19 14:39:31
tags:
---

docker deploy
https://docs.docker.com/engine/install/debian/

config apt source

```
echo \
"deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://mirrors.tuna.tsinghua.edu.cn/docker-ce/linux/debian \
$(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```
