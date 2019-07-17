---
layout: post
title: "How to fix suplibOsInit what: 3 VERR_VM_DRIVER_NOT_INSTALLED (-1908) "
date: 2017-04-06 13:32:20 +0300
description: "How to fix VirtualBox error suplibOsInit what: 3 VERR_VM_DRIVER_NOT_INSTALLED (-1908) " # Add post description (optional)
img:  vm-error.png # Add image post (optional)
tags: [Virtualbox, error,孙志刚]
---
Error when starting Virtualbox:
```
Kernel driver not installed (rc=-1908)

Make sure the kernel module has been loaded successfully.

where: suplibOsInit what: 3 VERR_VM_DRIVER_NOT_INSTALLED (-1908) - The support driver is not installed. On linux, open returned ENOENT.

```

### How to fix
https://forums.virtualbox.org/viewtopic.php?f=8&t=84092

解决办法：大多数问题都是通过Apple文档：![用户批准的内核扩展加载](https://developer.apple.com/library/content/technotes/tn2459/_index.html)来解决的。
综上所述：

* 如果安装失败，可能不会提示您转到“安全性”设置。没人知道它为什么会起作用/不起作用。
* 重新启动计算机，重试安装。
* 安装失败后，转到系统首选项»安全»常规，然后“允许Oracle”安装内核扩展。
* 重试安装。

