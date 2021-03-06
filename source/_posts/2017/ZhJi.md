---
title: 一次装机经历
date: 2017-11-06 23:32:21
tags: 随便水水

comments: true
---

最近很倒霉，电脑系统崩溃了，没办法，只能重装系统，把这次重装系统的经历写出来，当成纪念吧，也许以后再也不会有装Win7的经历了。

<!-- more -->

## 准备工作

这次装系统用的是光盘装系统，别问我为什么不用U盘，没多余的U盘了，在我手上的U盘特别容易坏。

具体看这个表就好

|   项目  |   配置  |
|:-----:|:-----:|
|   电脑  |   ThinkPad E431   |
|   系统  |   Win7旗舰版 |
|   安装介质    |   光盘  |
|   驱动  |   准备好网卡驱动 |

首先在I tell you上下载好Win镜像，然后使用软碟通烧录到光盘上。

**特别注明一下**，我用的是UEFI装机，光盘装机无所谓，但是使用U盘装机的，一定要注意一下，Win7镜像原生是不支持Uefi启动的，所以烧录之前需要对镜像稍微改动一下，需要在Win8以上（8、8.1、10）的镜像里提取EFI里的Boot文件夹，然后复制到win7镜像里，具体做法为：

> 复制Win10镜像里的efi\boot文件夹到Win7镜像相同位置。

![](https://i.loli.net/2017/11/07/5a0088c23365f.png)

## BIOS设置

以前我用的是Win10系统，如果不改变BIOS设置直接装机肯定是不行的。

首先是要关闭安全启动（Secuity Boot），然后打开CSM，不同品牌的主板设置会不一样。

![](https://i.loli.net/2017/11/07/5a008c1b2de14.jpg)

## 装机开始

首先开机按F12，进入启动选项，现在DVD启动，然后进入装机程序。接下来就是选择分区，格式化C盘，然后一步一步跟着走就好。

有洁癖的人可以使用PE去格式化和重新分区，我这里因为仅仅是重装系统，4K对齐在以前 就已经做好了，不需要重新做了。

注意一下，想做UEFI启动的话，硬盘必须使用GUID引导，GPT分区表，MBR是不行的。

##  激活系统

装机完成之后就是激活系统。因为是UEFI装机的Win7旗舰版，这就让激活增加了不少难度，以前经常用的KMS是行不通的，因为不是VL版，再更以前用的OEM也行不通，因为不是MBR分区表，网络上支持UEFI启动的激活工具少之又少。（我掏过钱的，别跟我提正版什么的，只是掏钱买的不想用罢了）。

## 安装驱动

装上最开始准备好的网卡驱动，然后到网上下载联想驱动安装程序，开始安装驱动。

**一定要在装机之前准备好网卡驱动**

## 更新系统

系统更新还是打开比较好，微软现在还仍然在给Win7打补丁，前一阵子的比特币勒索病毒，想想还是很害怕的。

## 重装软件

这是最蛋疼的一步了，软件什么的太多了，很多都要重装。

不过，到这一步就算是装机成功了。

装了一部分软件，赶紧更新一下博客看看。