---
title: 偶像大师-2 DISC 汉化补丁说明
author: AaronP
tags:
  - Tutorial
---

# 偶像大师2 汉化补丁 说明文档（Demo）

> 本文档为偶像大师2 PS3版（THE iDOLM@STER 2 \[BLJS10083\]） 汉化预览补丁 使用说明，本补丁目前只支持RPCS3模拟器或破解PS3实机体验，不支持Xbox360版本。
>
> 补丁包含本体与DLC内容汉化，目前还存在部分偶像的少数剧情或者DLC有缺译或错译；此外部分UI还未实现汉化，欢迎大家体验的同时进行捉虫或提供建议。
>
> 补丁与原版游戏存档兼容，但是可能原版游戏存档制作人的日语名称会在汉化版下显示不正确，部分歌曲的Live场景歌词可能存在简体中文汉字与日语汉字混用的情况。
>
> 补丁采用文件替换进行覆盖，需要更新补丁或还原原版游戏将被替换的文件重新用新文件或原版游戏文件覆盖即可，建议自行备份原版游戏文件。补丁支持RPCS3的超分辨率，目前暂对RPCS3模拟器的版本没有要求。

- [偶像大师2 汉化补丁 说明文档（Demo）](#%E5%81%B6%E5%83%8F%E5%A4%A7%E5%B8%882-%E6%B1%89%E5%8C%96%E8%A1%A5%E4%B8%81-%E8%AF%B4%E6%98%8E%E6%96%87%E6%A1%A3demo)
  - [安装原游戏与DLC](#%E5%AE%89%E8%A3%85%E5%8E%9F%E6%B8%B8%E6%88%8F%E4%B8%8Edlc)
  - [汉化覆盖](#%E6%B1%89%E5%8C%96%E8%A6%86%E7%9B%96)
    - [下载2代补丁](#%E4%B8%8B%E8%BD%BD2%E4%BB%A3%E8%A1%A5%E4%B8%81)
    - [覆盖文件](#%E8%A6%86%E7%9B%96%E6%96%87%E4%BB%B6)
      - [对于目录1](#%E5%AF%B9%E4%BA%8E%E7%9B%AE%E5%BD%951)
      - [对于目录2](#%E5%AF%B9%E4%BA%8E%E7%9B%AE%E5%BD%952)
      - [对于目录3](#%E5%AF%B9%E4%BA%8E%E7%9B%AE%E5%BD%953)
  - [模拟器其他问题](#%E6%A8%A1%E6%8B%9F%E5%99%A8%E5%85%B6%E4%BB%96%E9%97%AE%E9%A2%98)

## 安装原游戏与DLC

请自行获取游戏文件。如果使用RPCS3，可以参考OFA教程的[RPCS3说明](https://ofa.idolmaster.top/2025/07/18/InstallTutorial.html)

## 汉化覆盖

### 下载2代补丁

[腾讯微云](https://share.weiyun.com/SDJaXOmH)

打开链接，进入偶像大师2 PS3版目录，下载汉化补丁文件夹

![0](/images/patch_tut_0.png)

### 覆盖文件

打开RPCS3目录，找到类似以下3个目录，分别是

- 目录1：`dev_hdd0\game\BLJS10083DATA\USRDIR\resource`
- 目录2：`dev_hdd0\game\BLJS10083\USRDIR`
- 目录3：`games\THE iDOLM@STER 2 [BLJS10083]\PS3_GAME\USRDIR\resource`

其中目录1的`THE iDOLM@STER 2 [BLJS10083]`可能为你自己解压iso目录时的名字，可以任意。

![1](/images/patch_tut_1.png)

#### 对于目录1

打开下载补丁的`dev_hdd0>game>BLJS10083DATA>USRDIR`文件夹，一路点击进去到这个`resource`目录

![2](/images/patch_tut_2.png)

复制上面8个文件夹，拷贝到**目录1**，点击确定，全部替换。

![3](/images/patch_tut_3.png)

#### 对于目录2

打开下载补丁的`dev_hdd0>game>BLJS10083`文件夹，一路点击进去到这个USRDIR目录

![4](/images/patch_tut_4.png)

将`EBOOT.BIN`和`dlc/`文件夹复制，粘贴到**目录2，**点击确定，全部替换。

![5](/images/patch_tut_5.png)

#### 对于目录3

打开下载补丁的`games\THE iDOLM@STER 2 [BLJS10083]\PS3_GAME\USRDIR\resource`文件夹，全选

![6](/images/patch_tut_6.png)

全部粘贴到**目录3**，点击确定，全部替换。

![7](/images/patch_tut_7.png)

此时完成全部的汉化操作。后续如果有汉化更新，则将更新的补丁文件找到RPCS3游戏安装目录`dev_hdd0`中同名文件进行覆盖即可。

## 模拟器其他问题

RPCS3对于偶像大师2启动没有OFA稳定，有时会出现启动偶像大师2游戏时窗口黑屏，无法关闭的问题。此时需要强制关闭模拟器，并使用任务管理器（Windows快捷键 Ctrl+Alt+Delete ）等工具完全杀死模拟器进程，重新打开模拟器尝试启动，可能需要多次。

如果重试依旧黑屏，可以Configuration→CPU，将SPU Decoder选择为ASMJIT，Apply之后再尝试启动游戏，成功启动之后退出游戏，再改回LLVM启动游戏（ASMJIT性能不如LLVM，正常游戏时推荐依旧选择LLVM）

![8](/images/patch_tut_8.png)
