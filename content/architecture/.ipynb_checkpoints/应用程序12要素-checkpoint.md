# 应用程序12要素

# 介绍

在现代，软件通常作为服务交付：称为*Web 应用程序*或*软件即服务*。十二因素应用程序是一种构建软件即服务应用程序的方法，它：

- 使用**声明**格式进行设置自动化，以最大限度地减少新开发人员加入项目的时间和成本；
- 与底层操作系统有一个**干净的合同**，在执行环境之间提供**最大的可移植性；**
- 适合**部署**在现代**云平台上**，无需服务器和系统管理；
- **最大限度地减少**开发和生产之间的差异，实现**持续部署**以获得最大的敏捷性；
- 并且可以在不对工具、架构或开发实践进行重大更改的情况下进行**扩展。**

十二因素方法可以应用于以任何编程语言编写的应用程序，并使用支持服务（数据库、队列、内存缓存等）的任何组合。

# 背景

[本文档的贡献者直接参与了数百个应用程序的开发和部署，并通过我们在Heroku](http://www.heroku.com/)平台上的工作间接见证了数十万个应用程序的开发、运行和扩展。

本文档综合了我们对广泛使用的各种软件即服务应用程序的所有经验和观察。它是对应用程序开发理想实践的三角测量，特别关注应用程序随时间的有机增长动态、开发应用程序代码库的开发人员之间的协作动态，以及[避免软件侵蚀的成本](http://blog.heroku.com/archives/2011/6/28/the_new_heroku_4_erosion_resistance_explicit_contracts/)。

我们的动机是提高对我们在现代应用程序开发中看到的一些系统性问题的认识，为讨论这些问题提供一个共享的词汇表，并为这些问题提供一组广泛的概念性解决方案，并附带术语。该格式的灵感来自 Martin Fowler 的书籍*[Patterns of Enterprise Application Architecture](https://books.google.com/books/about/Patterns_of_enterprise_application_archi.html?id=FyWZt5DdvFkC)* and *[Refactoring](https://books.google.com/books/about/Refactoring.html?id=1MsETFPD3I0C)*。

# 谁应该阅读这份文件？

任何构建作为服务运行的应用程序的开发人员。部署或管理此类应用程序的运维工程师。

# 十二要素

## [一、代码库](https://12factor.net/codebase)

### 在修订控制中跟踪一个代码库，许多部署

## [二、依赖项](https://12factor.net/dependencies)

### 显式声明和隔离依赖项

## [三、配置](https://12factor.net/config)

### 在环境中存储配置

## [四。支持服务](https://12factor.net/backing-services)

### 将支持服务视为附加资源

## [五、构建、发布、运行](https://12factor.net/build-release-run)

### 严格分离构建和运行阶段

## [六、流程](https://12factor.net/processes)

### 将应用程序作为一个或多个无状态进程执行

## [七。端口绑定](https://12factor.net/port-binding)

### 通过端口绑定导出服务

## [八。并发](https://12factor.net/concurrency)

### 通过流程模型向外扩展

## [九。可处置性](https://12factor.net/disposability)

### 通过快速启动和正常关闭最大限度地提高鲁棒性

## [X. 开发/产品平价](https://12factor.net/dev-prod-parity)

### 保持开发、登台和生产尽可能相似

## [十一。日志](https://12factor.net/logs)

### 将日志视为事件流

## [十二。管理流程](https://12factor.net/admin-processes)

### 将管理/管理任务作为一次性流程运行
