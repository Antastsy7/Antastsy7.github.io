---
title: The Lost Book
comments: false
date: 2018-5-21
keywords: 
tags:
- TRPG
categories: Portfolio
description: 基于cocos的回合制游戏
photos: /assets/img/2018-5-21-The-Lost-Book/azhar.jpg
avatar: /assets/img/common/avatar.jpg
typora-root-url: ..
---

![azhar](/assets/img/2018-5-21-The-Lost-Book/azhar.jpg)

#### 游戏背景

Road Threader 是我们在 2019 年 9 月的Game Jam上设计制作的游戏。当时Game Jam的主题是逃离，而我们就联想到了逃离北上广，继而想到了北上广拥堵的交通，于是有了这个游戏的想法：通过给玩家超人一般的神速来让他们在堵车的路上横行无阻。

 

#### 设计思路

我们给游戏设计了随机刷新以及大小不一的车辆，玩家的车速会略慢于其他的车辆，因此需要用手在屏幕上拖拽滑动来让车辆在道路上快速穿梭，躲避即将撞上的车辆。拖拽的时候整个游戏世界的时间流逝会变慢，类似于子弹时间，玩家会有足够的时间来思考和规划路线。



#### 我的职责

我在这次项目中负责处理划线和碰撞的逻辑。用手指绘制线本身并不是很复杂，碰撞方面由于我们每次滑动时车速是不一样的，unity内置的物理引擎有时候会发生鬼畜的翻车，我们给车子特别做了各个角度翻车的动画，根据撞击的位置来选择对应的动画播放，让整体的撞击之后的效果更加可控一些。