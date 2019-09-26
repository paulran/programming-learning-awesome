# 从0开始学习计算机编程，需要知道哪些知识
## Contents
* [计算机组成原理](#计算机组成原理)
* [操作系统原理](#操作系统原理)
* [计算机网络](#计算机网络)
* [编程原理](#编程原理)
* [参考书](#参考书)



## 计算机组成原理
![](./images/computer-compose-principle_01.jpg)
## 操作系统原理
![](./images/operating-system_01.jpg)

操作系统主要包括以下几个方面的功能 ：
1. 进程管理：其工作主要是进程调度，在单用户单任务的情况下，处理器仅为一个用户的一个任务所独占， 进程管理的工作十分简单。但在多道程序或多用户的情况 下，组织多个作业或任务时，就要解决处理器的调度、 分配和回收等问题 。
2. 存储管理：存储分配、存储共享、存储保护 、存储扩张。
3. 设备管理：设备分配、设备传输控制 、设备独立性。
4. 文件管理：文件存储空间的管理、目录管理 、文件操作管理、文件保护。
5. 作业管理：负责处理用户提交的任何要求。

操作系统实例：
1. 嵌入式系统：
    1. 使用非常广泛的系统（如VxWorks、eCos、Symbian OS及Palm OS）以及某些功能缩减版本的Linux或者其他操作系统。某些情况下，OS指称的是一个内置了固定应用软件的巨大泛用程序。在许多最简单的嵌入式系统中，所谓的OS就是指其上唯一的应用程序。
    2. iOS是由苹果公司开发的手持设备操作系统。最初是设计给 iPhone 使用的，后来陆续套用到 iPod touch 、iPad 以及 Apple TV 等产品上。
    3. Android是一种基于Linux的自由及开放源代码的操作系统。主要使用于移动设备，如智能手机和平板电脑，由Google公司和开放手机联盟领导及开发。尚未有统一中文名称，中国大陆地区较多人使用“安卓”。
2. 类Unix系统：所谓的类Unix家族指的是一族种类繁多的OS，此族包含了System V、BSD与Linux。由于Unix是The Open Group的注册商标，特指遵守此公司定义的行为的操作系统。
3. 微软Windows：Microsoft Windows系列操作系统是在微软给IBM机器设计的MS-DOS的基础上设计的图形操作系统。现在的Windows系统，如Windows 2000、Windows XP皆是创建于现代的Windows NT内核。NT内核是由OS/2和OpenVMS等系统上借用来的。
4. MacOS：是一套运行于苹果Macintosh系列计算机上的操作系统，是一个从NeXTSTEP、Mach以及FreeBSD共同派生出来的微内核BSD系统。



## 计算机网络
分类：
1. 局域网：Local Area Network，LAN。   
![](./images/computer-network_02.jpg) 
2. 广域网：Wide Area Network，WAN。   
![](./images/computer-network_01.jpg)  

### TCP/IP协议
![](./images/tcp_ip_4tier_layer.png)  
* 应用层协议：如HTTP、FTP、SMTP、TELNET、DNS等  
* 链路层协议：如Ethernet和Wi-Fi  
![](./images/tcp_ip_lan.png)  
![](./images/tcp_ip_wan.png)  
* IP地址（IP Address）：
    - IP地址是IP协议提供的一种统一的地址格式，它为互联网上的每一个网络和每一台主机分配一个逻辑地址，以此来屏蔽物理地址的差异。
* 端口号（Port）：
    - 一台拥有IP地址的主机可以提供许多服务，比如Web服务、FTP服务、SMTP服务等，这些服务完全可以通过1个IP地址来实现。因为IP 地址与网络服务的关系是一对多的关系，不能只靠IP地址来区分不同的服务。实际上是通过“IP地址+端口号”来区分不同的服务的。
    - 客户端只需保证该端口号在本机上是惟一的就可以了。客户端端口号因存在时间很短暂又称临时端口号。
    - 一个IP地址的端口通过16bit进行编号，最多可以有65536个端口。端口是通过端口号来标记的，端口号只有整数，范围是从0 到65535。
* 域名（Domain Name）：
    - 是由一串用点分隔的名字组成的Internet上某一台计算机或计算机组的名称，用于在数据传输时标识计算机的电子方位（有时也指地理位置）。
    - 域名系统（DNS，Domain Name System）是因特网的一项核心服务，它作为可以将域名和IP地址相互映射的一个分布式数据库，是进行域名(domain name)和与之相对应的IP地址 (IP address)转换的系统，搭载域名系统的机器称之为域名服务器，能够使人更方便的访问互联网，而不用去记住能够被机器直接读取的IP地址数串。
* 路由器（Router）：
    - 是连接两个或多个网络的硬件设备，在网络间起网关的作用，是读取每一个数据包中的地址然后决定如何传送的专用智能性的网络设备。
    - ![](./images/network-route_01.png) 


## 编程原理
编辑可以让计算机执行的程序的过程就叫编程。  
计算机使用一种只包含1和0的简单语言，其中1表示“开”，0表示“关”。尝试用计算机自己的语言与其交谈就好像尝试用摩尔斯电报码与朋友交谈一样。  
编程语言相当于您和计算机之间的翻译。您不必学习计算机自己的语言(即“机器语言”)，而是可以使用编程语言，以一种更易于学习和理解的方式向计算机发出指令。一种称为“编译器”的专用程序接受用编程语言编写的指令。并将这些指令转换为机器语言。  

1. 解释程序：把源语言写的程序作为输入，但不产生目标程序，而是边解释边执行源程序本身。  
![](./images/interpreter_program.png)  
2. 编译程序：也称为编译器（Compiler），是指把用高级程序设计语言书写的源程序，翻译成等价的机器语言格式目标程序的翻译程序。  
![](./images/compiling_program.png)  
![](./images/compiling_process.png)  

### 网站架构设计
![](./images/server_design_02.png)  

### 网页浏览器
网页浏览器（英语：web browser），常被简称为浏览器，是一种用于检索并展示万维网信息资源的应用程序。这些信息资源可为网页、图片、影音或其他内容，它们由统一资源标志符标志。信息资源中的超链接可使用户方便地浏览相关信息。  
网页浏览器虽然主要用于使用万维网，但也可用于获取专用网络中网页服务器之信息或文件系统内之文件。  
主流网页浏览器有Mozilla Firefox、Internet Explorer、Microsoft Edge、Google Chrome、Opera及Safari。  
* 主要组件包括：  
    ![](./images/web_browser_compose.png)  
    1. 用户界面 － 包括地址栏、后退/前进按钮、书签目录等，也就是所看到的除了用来显示所请求页面的主窗口之外的其他部分。  
    2. 浏览器引擎 － 用来查询及操作渲染引擎的接口。  
    3. 渲染引擎 － 用来显示请求的内容，例如，如果请求内容为html，它负责解析html及css，并将解析后的结果显示出来。  
    4. 网络 － 用来完成网络调用，例如http请求，它具有平台无关的接口，可以在不同平台上工作。  
    5. UI后端 － 用来绘制类似组合选择框及对话框等基本组件，具有不特定于某个平台的通用接口，底层使用操作系统的用户接口。  
    6. JS解释器 － 用来解释执行JS代码。  
    7. 数据存储 － 属于持久层，浏览器需要在硬盘中保存类似cookie的各种数据，HTML5定义了web database技术，这是一种轻量级完整的客户端存储技术。  


## 参考书
1. 《TCP/IP协议详解》，卷1和卷2。
2. 《C程序设计语言第二版·新版》 ，作者(美)克尼汉（Brian W. Kernighan） 、(美)里奇（Dennis M. Ritchie），翻译徐宝文、 李志，2004年01月机械工业出版社出版。本书全面、系统地讲述了C语言的各个特性及程序设计的基本方法,包括基本概念、类型和表达式、控制流、函数与程序结构、指针与数组、结构、输入与输出、UNIX系统接口、标准库等内容。
3. 《自己动手写操作系统》由电子工业出版社于2005年8月发行，作者是 于渊。本书主要介绍如何用C语言和汇编语言编写出具备操作系统基本功能的操作系统框架。
4. 《OrangeS：一个操作系统的实现》是2009年6月1日电子工业出版社 出版的图书，作者是于渊。本书从只有二十行的引导扇区代码出发，一步一步地向读者呈现一个操作系统框架的完成过程。书中不仅关注代码本身，同时关注完成这些代码的思路和过程。本书不同于其他的理论型书籍，而是提供给读者一个动手实践的路线图。读者可以根据路线图逐步完成各部分的功能，从而避免了一开始就面对整个操作系统数万行代码时的迷茫和挫败感。书中讲解了大量在开发操作系统中需注意的细节问题，这些细节不仅能使读者更深刻地认识操作系统的核心原理，而且使整个开发过程少走弯路。
5. 《30天自制操作系统》是2012年人民邮电出版社出版的图书，作者是川合秀实。这是一本兼具趣味性、实用性与学习性的书籍。作者从计算机的构造、汇编语言、C语言开始解说，让你在实践中掌握算法。在这本书的指导下，从零编写所有代码，30天后就可以制作出一个具有窗口系统的32位多任务操作系统。

  
