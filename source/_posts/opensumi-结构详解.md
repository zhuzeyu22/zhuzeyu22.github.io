---
title: opensumi 结构详解
date: 2023-11-28 09:33:55
tags:
---

# 插件

两个入口点
extensionEntry
extensionWorkerEntry

由 MainApp 启动
ElectronMainApp

MainApp 包含
codeWindows
injector
modules
parsedArgs

注册 api
injectLifecycleApi


``` ts
// 很优秀的类型推断，判断 T 是推断类型 R 的实例类型
export type TokenResult<T extends Token> = T extends ConstructorOf<infer R> ? R : any;
```

初始化的时候发出事件
ActivationEventServiceImpl



export class BasicModule {
  @Autowired(INJECTOR_TOKEN)
  protected injector: Injector;
  providers?: Provider[];
  backServices?: BackService[];
  frontServices?: FrontService[];
  contributionProvider: Domain | Domain[];
}

# 配置项注册
this.schemaRegistry.registerSchema