# Guava的使用

[TOC]

## 参考资料

| 资料名称      | 来源                                                         |
| ------------- | ------------------------------------------------------------ |
| Guava官方教程 | https://wizardforcel.gitbooks.io/guava-tutorial/content/1.html |
|               |                                                              |
|               |                                                              |



## Guava介绍

Guava是Google的一组核心Java类库，其中包括新的集合类型、图形库以及用于并发、I/O、哈希、缓存、字符串等实用工具类，广泛用于Google的大多数项目中，并且被许多公司使用。

Guava工程包含了若干被Google的 Java项目广泛依赖 的核心库，例如：集合 [collections] 、缓存 [caching] 、原生类型支持 [primitives support] 、并发库 [concurrency libraries] 、通用注解 [common annotations] 、字符串处理 [string processing] 、I/O 等等。 



## 功能简介

如下是官网提供的Guava完整功能介绍目录。本文主要探究Guava中提供的集合处理、EventBus消息总线、Guava Cache单机缓存、异步回调工具listenableFutrue以及重试机制。

### 基本工具 [Basic utilities]

让使用Java语言变得更舒适

- [使用和避免null](http://ifeve.com/using-and-avoiding-null/)：null是模棱两可的，会引起令人困惑的错误，有些时候它让人很不舒服。很多Guava工具类用快速失败拒绝null值，而不是盲目地接受

- [前置条件](http://ifeve.com/google-guava-preconditions/): 让方法中的条件检查更简单

- [常见Object方法](http://ifeve.com/google-guava-commonobjectutilities/): 简化Object方法实现，如hashCode()和toString()

- [排序: Guava强大的”流畅风格比较器”](http://ifeve.com/google-guava-ordering/)

- [Throwables](http://ifeve.com/google-guava-throwables/)：简化了异常和错误的传播与检查

### 集合[Collections]

Guava对JDK集合的扩展，这是Guava最成熟和为人所知的部分

- [不可变集合](http://ifeve.com/google-guava-immutablecollections/): 用不变的集合进行防御性编程和性能提升。

- [新集合类型](http://ifeve.com/google-guava-newcollectiontypes/): multisets, multimaps, tables, bidirectional maps等

- [强大的集合工具类](http://ifeve.com/google-guava-collectionutilities/): 提供java.util.Collections中没有的集合工具

- [扩展工具类](http://ifeve.com/google-guava-collectionhelpersexplained/)：让实现和扩展集合类变得更容易，比如创建`Collection`的装饰器，或实现迭代器

### [缓存](http://ifeve.com/google-guava-cachesexplained)[Caches]

Guava Cache：本地缓存实现，支持多种缓存过期策略

### [函数式风格](http://ifeve.com/google-guava-functional/)[Functional idioms]

Guava的函数式支持可以显著简化代码，但请谨慎使用它

### 并发[Concurrency]

强大而简单的抽象，让编写正确的并发代码更简单

- [ListenableFuture](http://ifeve.com/google-guava-listenablefuture/)：完成后触发回调的Future

- [Service框架](http://ifeve.com/google-guava-serviceexplained/)：抽象可开启和关闭的服务，帮助你维护服务的状态逻辑

### [字符串处理](http://ifeve.com/google-guava-strings/)[Strings]

非常有用的字符串工具，包括分割、连接、填充等操作

### [原生类型](http://ifeve.com/google-guava-primitives/)[Primitives]

扩展 JDK 未提供的原生类型（如int、char）操作， 包括某些类型的无符号形式

### [区间](http://ifeve.com/google-guava-ranges/)[Ranges]

可比较类型的区间API，包括连续和离散类型

### [I/O](http://ifeve.com/google-guava-io/)

简化I/O尤其是I/O流和文件的操作，针对Java5和6版本

### [散列](http://ifeve.com/google-guava-hashing/)[Hash]

提供比`Object.hashCode()`更复杂的散列实现，并提供布鲁姆过滤器的实现

### [事件总线](http://ifeve.com/google-guava-eventbus/)[EventBus]

发布-订阅模式的组件通信，但组件不需要显式地注册到其他组件中

### [数学运算](http://ifeve.com/google-guava-math/)[Math]

优化的、充分测试的数学工具类

### [反射](http://ifeve.com/guava-reflection/)[Reflection]

Guava 的 Java 反射机制工具类



## 导入Guava依赖

```
<dependency>
  <groupId>com.google.guava</groupId>
  <artifactId>guava</artifactId>
  <version>29.0-jre</version>
</dependency>
```



## 集合处理





## EventBus消息总线





## Guava Cache单机缓存





## 并发listenableFutrue回调





## 重试机制

