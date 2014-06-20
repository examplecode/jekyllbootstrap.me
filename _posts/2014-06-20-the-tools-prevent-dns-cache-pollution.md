---
layout: post
title: "防止DNS污染的小工具"
description: "一个小工具用于返回被GFW污染的真实域名"
category: tools
tags: [gfw,dns,tools]
---
{% include JB/setup %}

以前写的小工具，最近整理代码，再这里公布出来。这个小工具用于获取被gfw dns 污染域名的真实ip地址，通常可以用于获取twitter,youtube,facebook等网址的真实ip地址。如果你的某些程序需要绕过GFW DNS污染也许这些代码片断会用的上，分别提供了c语言和java的实现版本。

[前往 github 源码地址][1]

## C 语言版本

### 编译

    gcc -o gfw_dns_resolver  gfw_dns_resolver.c 

编译输出调试信息版本
    
    gcc -o gfw_dns_resolver -DDEBUG gfw_dns_resolver.c 


### 运行示例

    ./gfw_dns_resolver www.twitter.com

输出:

    The real ip is: 199.59.149.230


## JAVA 版本

### 编译

    javac GFWDnsResolver.java

### 运行示例
    java GFWDnsResolver www.youtube.com

输出：

    host:www.youtube.com The real ip is:173.194.72.102


[前往 github 源码地址][1]

[1]: https://github.com/examplecode/gfw_dns_resolver