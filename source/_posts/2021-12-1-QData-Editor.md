---
title: 2021-12-1-QData-Editor
author: slakijng
avatar: \assets\img\common\avatar.jpg
authorDesc: 一个好奇的人
categories: 技术
comments: false
date: 2022-06-29 13:01:51
authorLink:
authorAbout:
tags:
keywords:
description:
photos:
---
## 项目概述
我们项目绝大部分数据都存在表格里，一个数据要在游戏中生效需要编辑后走一遍导表流程，不仅过程繁长，是否生效了也处于薛定谔状态。因此我们希望有一个可以快速查询服务器数据的工具，再进一步拓展可以快速修改服务器数据。
## 设计思路
我们项目已经有一个reload函数，用于导表后重新加载数据并在游戏中生效。同时我们每个游戏数据data文件都会对应一个def文件，记录了这个data是由哪(些)个excel表格文件导表而来，每个字段分别被映射到哪个新的字段上。
## 