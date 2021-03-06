# Java EE Fundamentals – Microservices

#  5. Microservices - JavaEE基础系列

This is the fifth post in the [Java EE](https://is.gd/theoryee) Fundamentals series

本文是JavaEE基础系列的第五节。

1. [Java EE简介 - JavaEE基础系列](http://blog.csdn.net/renfufei/article/details/74073705)
2. [JSR简介 - JavaEE基础系列](http://blog.csdn.net/renfufei/article/details/74074616)
3. [什么是JSR参考实现？ - JavaEE基础系列](http://blog.csdn.net/renfufei/article/details/74094488)
4. [4. 什么是应用服务器？ - JavaEE基础系列](http://blog.csdn.net/renfufei/article/details/74723946)



[Microservices](https://en.wikipedia.org/wiki/Microservices) is the latest software architecture that seems to be the buzzword of the day. It has been around in[ one form](https://en.wikipedia.org/wiki/Service-oriented_architecture) or the other since the early days of software engineering.

[Microservices,微服务](https://en.wikipedia.org/wiki/Microservices) 是当今世界上最火爆的软件开发架构。相对于早期的软件工程来说, 微服务已成为了一种新形式的 [面向服务的架构(SOA)](https://en.wikipedia.org/wiki/Service-oriented_architecture) 。

Essentially microservices means breaking down applications into distinct components that all coordinate to form a whole. Now there are arguments against Java EE given it’s application server centric nature. There are those that think Java EE is heavy and geared towards the monolith style of application development.

微服务本质上是将系统拆分成多个不同的组件, 互相之间协调组合成一个整体。 现在有一种说法, 认为Java EE 应用服务器不再是Java生态的核心。原因是 Java EE 太笨重了, 只适合开发单体应用程序。

However, this is very incorrect. In fact, Java EE is more than suitable for a microservices architecture. At its core, microservices basically means an application being self-contained in terms of its runtime dependencies. Meaning generally the application has a small footprint and can theoretically be deployed to almost any usable platform.

但这种说法其实是有问题的, Java EE 也非常适用于微服务架构开发. 最最核心的地方, 微服务的运行时是自包容的(self-contained), 代码和依赖都在一起. 同时,微服务占用空间小, 理论上,可以部署到任何平台。

Java EE has tools available that make it super easy to create a microservices oriented application with it. The following 4 tools are more than enough to create any kind of microservices with Java EE.

有很多支持 Java EE 的工具, 可以简单快速地创建面向微服务的应用。下面是4种常见的微服务创建工具。

# **Payara Micro**


[Payara Micro](https://www.payara.fish/payara_micro) is a microservices geared version of the popular, open source, Glassfish derived Payara Server. Payara Micro is designed for running Java EE applications in a modern containerized / virtualized infrastructure, using automated provisioning tools like Chef, Ansible or Puppet. Payara Micro makes it easy to java -jar your Java EE application.

[Payara Micro](https://www.payara.fish/payara_micro) 基于 Glassfish 开发, 是一款开源的 microservices 创建工具, 当前处于 geared 版本. Payara Micro 是专为容器/虚机环境设计的, 支持多种配置管理工具, 如Chef, Ansible 和 Puppet 等. Payara Micro 可以非常简单地使用 ·java -jar· 方式运行 Java EE 应用。

# **JBoss Wildfly Swarm**


[WildFly Swarm](http://wildfly-swarm.io/) offers an innovative approach to packaging and running Java EE applications by packaging them with just enough of the server runtime to “java -jar” your application. Essentially it bundles your Java EE dependencies with your application making your resulting war/jar self contained.

[WildFly Swarm](http://wildfly-swarm.io/) 提供了一种全新的方法来包装和运行Java EE 应用, 通过 “java -jar” 的方式即可执行服务器运行时. 本质上, 是将 Java EE 依赖整体打包到一起, 使得应用程序 `war/jar` 自包含(self contained)。

# **KumuluzEE**


[KumuluzEE](https://ee.kumuluz.com/) is a lightweight open-source microservice framework. It’s raison d’être is to help you develop microservices with Java EE technologies and also migrate existing Java EE applications to a microservices architecture.

[KumuluzEE](https://ee.kumuluz.com/) 是一框轻量级的开源微服务框架. 它存在的目的, 是为了帮助 Java EE 程序员开发 微服务,以及将现有的Java EE应用迁移到microservices架构中。

# **Apache Meecrowave 服务**


[Apache Meecrowave](http://openwebbeans.apache.org/meecrowave/index.html#) is a lightweight JAX-RS, CDI and JSON server.  Meecrowave is suitable for developing microservices using the mentioned Java EE APIs. In fact, the CDI runtime that powers Meecrowave – OpenWebBeans – recently became[ CDI 2.0 (JSR 365)](https://is.gd/ee7cdi)compatible.

[Apache Meecrowave](http://openwebbeans.apache.org/meecrowave/index.html) 是一款轻量级的  JAX-RS, CDI and JSON 服务器. Meecrowave 适合于 mentioned 方式开发微服务。事实上,CDI运行时支撑了 Meecrowave - OpenWebBeans 最近兼容 [CDI 2.0 (JSR 365)](https://is.gd/ee7cdi)。

In subsequent posts, we will be taking all these tools one after the other and examine them in detail complete with code samples.

在后续文章中,我们将一次介绍这些工具, 并通过代码对他们进行详细讲解。


原文日期: 2017年7月23日

原文链接: <https://pedanticdevs.com/2017/07/java-ee-fundamentals-microservices.html>

翻译日期: 2017年7月28日

翻译人员: [铁锚: http://blog.csdn.net/renfufei](http://blog.csdn.net/renfufei)

