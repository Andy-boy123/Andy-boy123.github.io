---
layout:       post
title:        "一些名词"
author:       "Andy"
header-style: text
catalog:      true
tags:
    - words
    - study
---

#### 1. 什么是**协程**?
> 协程是一种比线程更加轻量级的存在，协程的调度完全由用户控制。协程拥有自己的寄存器上下文和栈。协程调度切换时，将寄存器上下文和栈保存到其他地方，切换回来的时候，恢复先前保存的寄存器上下文和栈。

#### 2. 什么是**线程**?
> 线程是操作系统能够进行运算调度的最小单位。它被包含在进程之中，是进程中的实际运作单位。一个进程可以由很多个线程组成，线程间共享进程的所有资源，每个线程有自己的堆栈和局部变量。线程由CPU独立调度执行，在多CPU环境下就允许多个线程同时运行。同样多线程也可以实现并发操作，每个请求分配一个线程来处理。

#### 3. 什么是**进程**?
> 进程是指在系统中正在运行的一个应用程序。每个进程之间是独立的、不可交互的。进程也是程序的一次执行过程，是系统运行程序的基本单位，因此进程是动态的。系统运行一个程序即是一个进程从创建、运行到消亡的过程。

#### 4. 什么是**协议**?
> 协议是指计算机通信或网络通信中两台计算机之间进行通信所必须共同遵守的规定或规则。协议包括语法、语义和同步三个层面。语法层面是指协议中的数据格式，即数据应该以怎样的形式出现；语义层面是指协议中的控制信息，即数据应该怎样流动；同步层面是指协议中的事件顺序，即数据应该什么时候出现。

#### 5. 什么是**TCP/IP**?
> TCP/IP是指传输控制协议/因特网互联协议，是Internet最基本、最广泛的协议。TCP/IP协议族是一个层次化的协议集合，共分为四层：链路层、网络层、传输层和应用层。

#### 6. 什么是**HTTP**?
> HTTP是指超文本传输协议，是一种详细规定了浏览器和万维网服务器之间互相通信的规则，通过因特网传送万维网文档的数据传送协议。HTTP协议通常承载于TCP协议之上，有时也承载于TLS或SSL协议层之上，这个时候，就成了我们常说的HTTPS。

#### 7. 什么是**HTTPS**?
> HTTPS是指超文本传输安全协议，是一种通过计算机网络进行安全通信的传输协议。HTTPS经由HTTP进行通信，但利用SSL/TLS来加密数据包。HTTPS开发的主要目的，是提供对网站服务器的身份认证，保护交换数据的隐私与完整性。

#### 8. 什么是**SSL**?
> SSL是指安全套接字层，是为网络通信提供安全及数据完整性的一种安全协议。SSL协议位于TCP/IP协议与各种应用层协议之间，为数据通讯提供安全支持。SSL协议可分为两层：SSL记录协议和SSL握手协议。

#### 9. 什么是**TLS**?
> TLS是指传输层安全协议，是一种安全的传输协议。

#### 10. 什么是**IP**?
> IP是指互联网协议，是一种网络协议，用于把数据包从源地址传送到目的地址。IP协议为数据包的传输打下了基础，它定义了数据包的格式、传送方式、路由方式等等。

#### 11. 什么是**TCP**?
> TCP是指传输控制协议，是一种面向连接的、可靠的、基于字节流的传输层通信协议，由IETF的RFC 793定义。在简化的计算机网络OSI模型中，它完成第四层传输层所指定的功能。用户数据报协议（UDP）是同一层内另一个重要的传输协议。

#### 12. 什么是**UDP**?
> UDP是指用户数据报协议，是OSI（Open System Interconnection，开放式系统互联）参考模型中一种无连接的传输层协议，提供面向事务的简单不可靠信息传送服务。UDP不提供可靠性，它只是把应用程序传给IP层的数据报发送出去，但是并不能保证它们能到达目的地。由于UDP在传输数据报前不用在客户和服务器之间建立一个连接，且没有超时重发等机制，故而传输速度很快。

#### 13. 什么是**DNS**?
> DNS是指域名系统，是一种组织成域层次结构的计算机和网络服务命名系统，它用于TCP/IP网络，它所提供的服务是用来将主机名和域名转换为IP地址的工作。DNS提供的是一种用来方便地访问计算机和服务的机制，它实际上是一个大型的分布式数据库，能够让用户利用域名来查询特定主机的IP地址信息。

#### 14. 什么是**资源**?
>所谓的资源就是网络上的一个实体，它可以使一个图片，一个文本，一个服务，你可以用一个URI指向它，每种资源对应一个特定的URI，要获取这个资源访问它的URI就行了，所谓的上网，其实就是与网络上的资源进行一系列的互动就是了。

#### 15. 什么是**URI**?
>URI是指统一资源标识符，是用于标识某一互联网资源名称的字符串，是一种用于标识某一互联网资源名称的字符串，是一种用于标识某一互联网资源的名称的字符串，包含了用于定位它的一系列的信息，但是不指定如何定位以及如何访问。URI包括URL和URN两种，URL是统一资源定位符，是一种具体的URI，它是一种定位资源的手段，而不是一种资源；URN是统一资源名称，是通过名字来标识资源。

#### 16. 什么是**URL**?
>URL是指统一资源定位符，是一种具体的URI，它是一种定位资源的手段，而不是一种资源，它的作用是指定了一个资源的特定位置，它是一种具体的URI，包含了用于定位它的信息，如访问资源所需的网络协议等。

#### 17. 什么是**状态转移**?
>状态转移是指客户端和服务器之间的一系列请求和响应的过程，其中每一个请求都必须包含足够的信息以便服务器理解这个请求，并且能够理解这个请求的含义，而服务器则返回足够多的信息以便客户端去理解这个响应。

#### 18. 什么是**表征**?
>表征是指客户端和服务器之间传送的资源的某一种具体表现形式，可以是图片、文本、视频等等。

#### 19. 什么是**表征状态转移**?
>表征状态转移是指客户端和服务器之间传送的资源的某一种具体表现形式，可以是图片、文本、视频等等。

#### 20. 什么是**WSGI**?
>WSGI是指Web Server Gateway Interface，是一种规范，它定义了Web服务器与Web应用程序之间或框架之间的简单而通用的接口，WSGI的其中一个目的就是让用户可以用相同的方式编写前端和后端，而不用关心服务器或者框架的具体实现。