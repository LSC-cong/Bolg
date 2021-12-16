## 基础重点(必须扎实)

### Java语言

- 语言基础 **《Java核心技术》**
  - 基础语法
  - 面向对象
  - 常用API
  - 异常处理
  - 集合
  - IO
  - 多线程
  - 网络编程
  - 泛型
  - 反射
  - 注解
- JVM **《深入理解Java虚拟机》**
  - 类加载机制
    - 双亲委托
  - 字节码执行机制
  - JVM内存模型
    - 堆区
    - 虚拟机栈
    - 方法区
  - GC垃圾回收
  - JVM性能监控与故障定位
  - JVM调优
- 多线程、锁、并发 **1:《Java并发编程的艺术》、2:《Java并发编程实战》**
  - 并发编程基础
  - 线程池
  - 锁
    - 乐观锁、悲观锁
    - 互斥锁、共享锁
    - 可重入锁、偏向锁
    - 轻量级锁、CAS与自旋锁
  - 并发容器
  - 原子类
  - JUC并发工具类
- 网络编程
  - 学习路径
    - Socket API + 多线程 + 网络模型/IO模型 + IO复用
    - Netty
  - 核心点
    - 进程间通信方式：信号量、管道、共享内存、socket 等
    - 多线程编程：互斥锁、条件变量、读写锁、线程池等
    - 五大 IO 模型：同步、异步、阻塞、非阻塞、信号驱动
    - 高性能 IO 两种模式：Reactor 和 Proactor
    - IO 复用机制：epoll、select、poll（破解 C10K 问题的利器）
- Java源码

### 数据库/SQL

- **《SQL必知必会》、《高性能MySQL》**
- SQL语句
  - 手写SQL
    - 联表
    - 聚合
- SQL语句优化
- 事务、隔离级别
- 索引
- 锁

### 数据结构与算法

- **《漫画算法》、《算法》**
- 数据结构
  - 字符串
  - 数组
  - 链表
  - 栈
  - 队列
  - 二叉树
  - 堆
  - 哈希
- 算法
  - 十大排序
  - 查找、二分
  - 贪心
  - 分治
  - 动态规划
  - 回溯

### 设计模式

- **《重学Java设计模式》**
- 单例
- 工厂
- 代理
- 策略
- 模板方法
- 观察者
- 适配器
- 责任链
- 建造者
- 。。。。

### 计算机网络

- **《计算机网络：自顶向下方法》**
- HTTP、TCP、IP、ICMP、UDP、DNS、ARP
- IP地址、MAC地址、OSI七层模型（或者 TCP/IP 五层模型）
- HTTPS安全相关的：数字签名、数字证书、TLS
- 常见网络攻击：局域网ARP泛洪、DDoS、TCP SYN Flood、XSS等
- TCP协议（最重要）
  - TCP协议
    - 三次握手、四次挥手
    - 状态转换
    - TCP状态中TIME_WAIT
    - 拥塞控制
    - 快速重传、慢启动
  - 问题
    - TCP 如何实现可靠传输的（画外音：如何基于 UDP 实现可靠传输）
    - TCP 连接建立为什么不是两次握手（画外音：三次握手的充分必要性说明）
    - TIME_WAIT 的存在解决了什么问题，等待时间为什么是 2 MSL
  - 核心
    - 可靠传输 + 高效传输（流量控制和窗口管理）
- HTTP、HTTPS
  - 从 URL 输入到页面展现到底发生什么
- **学习方法**
  - 学习抓住一条主线
    - 一个数据包是如何发送出去的
  - 带着问题去思考为什么这么做

### 操作系统

- **《现代操作系统》**
- 进程管理
- 并发、同步互斥、锁
- 内存管理
- 文件系统
- 重点
  - OS四大模块的理论知识
    - 进程与线程管理
    - 内存管理
    - IO与文件系统
    - 设备管理
  - 了解Linux内核部分实现原理
    - 内存管理
    - 进程管理
    - 虚拟文件系统
  - 与编程最密切
    - 内存
    - 进程
    - IO
- 认知
  - 操作系统由哪些构成
  - 进程的状态、切换、调度
  - 进程间通信方式（共享内存、管道、消息）
  - 进程和线程的区别
  - 线程的实现方式（一对一、多对一等）
  - 互斥与同步（信号量、管程、锁）
  - 死锁检测与避免
  - 并发经典的问题：读者写者、哲学家就餐问题
  - 为什么需要虚拟内存，MMU 具体如何做地址转换的
  - 内存为什么分段、分页
  - 页面置换算法
  - 文件系统是如何组织的
  - 虚拟文件系统（VFS）是如何抽象的
  - 。。。。

## 应用框架

### 后端

- JSP、Servlet
- Spring家族
  - Spring
    - IOC
    - AOP
  - Spring MVC
  - MyBatis
  - SSM
    - 打war包
    - Tomcat运行
  - Spring Boot
    - 打jar包
      - 内嵌Tomcat
        - 微服务架构
    - 知识点
      - 自动配置、开箱即用
      - 整合Web
      - 整合数据库（事务问题）
      - 整合权限
        - Shiro
        - SpringSecurity
      - 各种中间件
        - 缓存
        - MQ
        - RPC框架
          - Dubbo
        - NIO框架
          - Netty
  - Spring Cloud
    - Netflix
      - Eureka
        - 服务治理组件，包括服务端的注册中心和客户端的服务发现机制。
      - Ribbon
        - 负载均衡的服务调用组件，具有多种负载均衡调用策略。
      - Hystrix
        - 服务容错组件，实现了断路器模式，为依赖服务的出错和延迟提供了容错能力。
      - Feign
        - 基于Ribbon和Hystrix的声明式服务调用组件。
      - Zuul
        - API 网关服务，过滤、安全、监控、限流、路由。
    - Alibaba
      - Nacos
        - 阿里巴巴开源产品，一个更易于构建云原生应用的动态服务发现、配置管理和服务管理平台。
      - Sentinel
        - 面向分布式服务架构的轻量级流量控制产品，把流量作为切入点，从流量控制、熔断降级、系统负载保护等多个维度保护服务的稳定性。
      - RocketMQ
        - 一款开源的分布式消息系统，基于高可用分布式集群技术，提供低延时的、高可靠的消息发布与订阅服务。
      - Dubbo
        - Apache Dubbo 是一款高性能 Java RPC 框架，用于实现服务通信。
      - Seata
        - 阿里巴巴开源产品，一个易于使用的高性能微服务分布式事务解决方案。
    - Config
      - 分布式配置中心。配置管理工具，支持使用 Git 存储配置内容，支持应用配置的外部化存储，支持客户端配置信息刷新、加解密配置内容等。
    - Bus
      - 事件、消息总线，用于在集群（例如，配置变化事件）中传播状态变化，可与 Spring Cloud Config 联合实现热部署。
    - Consul
      - 服务注册和配置管理中心。
    - Security
      - 安全工具包，对Zuul代理中的负载均衡OAuth2客户端及登录认证进行支持。
    - Sleuth
      - SpringCloud应用程序的分布式请求链路跟踪，支持使用Zipkin、HTrace和基于日志（例如ELK）的跟踪。
    - Stream
      - 轻量级事件驱动微服务框架，可以使用简单的声明式模型来发送及接收消息，主要实现为Apache Kafka及RabbitMQ。
    - Task
      - 用于快速构建短暂、有限数据处理任务的微服务框架，用于向应用中添加功能性和非功能性的特性。
    - Zookeeper
      - 服务注册中心。
    - Gateway（可替代 Zuul）
      - Spring Cloud Gateway 是 Spring 官方基于 Spring 5.0，Spring Boot 2.0 和 Project Reactor 等技术开发的网关，Spring Cloud Gateway 旨在为微服务架构提供一种简单而有效的统一的 API 路由管理方式。Spring Cloud Gateway 作为 Spring Cloud 生态系中的网关，目标是替代 Netflix Zuul，其不仅提供统一的路由方式，并且基于 Filter 链的方式提供了网关基本的功能，例如：安全，监控/埋点，和限流等。
    - OpenFeign（可替代 Feign）
      - OpenFeign 是 Spring Cloud 在 Feign 的基础上支持了 Spring MVC 的注解，如 [@RequesMapping](https://github.com/RequesMapping)等等。OpenFeign 的 [@FeignClient](https://github.com/FeignClient) 可以解析 SpringMVC 的 [@RequestMapping](https://github.com/RequestMapping) 注解下的接口，并通过动态代理的方式产生实现类，实现类中做负载均衡并调用其他服务。
  - 项目经验
    - 总结
- 中间件
  - 缓存
    - Redis
      - 5大数据类型
      - 事务
      - 消息通知
      - 管道
      - 持久化
      - 集群
  - 消息
    - RabbitMQ
    - RocketMQ
    - Kafka
  - 搜索
    - ElasticSearch

### 前端

- 基础套餐
  - 三大件
    - HTML
    - CSS
    - JavaScript
  - 基础库
    - jQuery
    - Ajax
- 模板框架
  - JSP
  - Thymeleaf
  - FreeMaker
- 组件化框架
  - Node
  - VUE
  - React
  - Angular

## 开发工具

### 集成开发环境

- Eclipse
- IDEA
- VSCode

### Linux系统

- Linux常用命令
- 基本Shell脚本

### 代码管理工具

- Git
  - Git命令和使用
- SVN

### 项目管理/构建工具

- Maven
- Gradle

## 应用运维

### Web服务器

- Nginx

### 应用服务器

- Tomcat

### 容器技术

- Docker
- Kubernetes(K8S)
  - 管理运维容器

### 持续集成、持续发布

- Jenkins

### 代码质量检测

- Sonar

### 日志收集、分析

- ELK

### CDN加速