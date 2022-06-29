---
title: The Lost Book
comments: false
date: 2018-5-21
keywords: 
tags:
- TRPG
categories: Demo
description: 基于cocos的回合制游戏
photos: /assets/img/2018-5-21-The-Lost-Book/azhar.jpg
avatar: /assets/img/common/avatar.jpg
typora-root-url: ..
---

#### 游戏背景

这是我在本科时第一次制作游戏，当时使用的引擎是cocos。

#### 设计思路

由于我们几个朋友都比较喜欢火焰纹章，于是就想做一个类似的TRPG游戏。我们给这个游戏设定了一个类似火纹的完整世界观与剧情框架（以及一长串中二到不行的名字）几个主角也都有了画稿。我们基本完成了序章，但是由于画师跑路也没有继续进行下去。

![20190808212950](/assets/img/2018-5-21-The-Lost-Book/20190808212950.jpg)

#### 我的职责

我负责所有的UI界面表现，战斗逻辑由我的另一个朋友负责。做的界面大致有：对话框、游戏地图、人物属性、战斗界面，以及一些飘窗提示、菜单等等。我们基本上做到了界面与逻辑分离，这样的好处是很多的，比如我在显示角色高亮范围的时候不，只需要按map_controler给我的结果染色即可。战斗时的演示也是先计算好结果再播一遍动画，这样的管线更加高效。

由于这是我做的第一个游戏项目，很多概念我都不太熟悉，比如在切场景时没有设一个scenemanager，而是用各种古怪的callback function来进行界面直接的来回调用。虽然当时项目还不复杂还可以接受，但这样的结构无疑拓展性很差且难以维护，这也让我后来的制作中意识到了各种manager的重要性。