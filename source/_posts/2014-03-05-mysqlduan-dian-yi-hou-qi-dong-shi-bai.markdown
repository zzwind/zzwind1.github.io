---
layout: post
title: "Mysql断电以后启动失败"
date: 2014-03-05 14:03:11 +0800
comments: true
categories: Mysql 
---
服务器停电以后,Mysql服务器一直启动不起来.总监以为是系统文件出问题了.
结果是Mysql启动程序会检测pid文件。如果pid文件存在就认为Mysql程序在运行中.
解决办法就是Delete pid file!Restart mysql successful!
