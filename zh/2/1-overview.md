---
title: Lesson 2 Overview
actions: ['checkAnswer', 'hints']
material:
  saveZombie: false
  zombieBattle:
    zombie:
      lesson: 1
    humanBattle: true
    ignoreZombieCache: true
    answer: 1
---

在第一课中，我们创建了一个命名函数用来生成僵尸，并且将它放入区块链上的僵尸数据库中。
在第二课里，我们会让我们的app看起来更像一个游戏： 它得支持多用户，并且采用更加有趣--而不仅仅随机--的方式，来生成新的僵尸。

如何生成新的僵尸呢？通过让现有的僵尸猎食其他生物！

## 僵尸猎食

僵尸猎食的时候， 僵尸病毒侵入猎物， 这些病毒会将猎物变为新的僵尸，加入你的Solidity。系统会通过猎物和猎食者僵尸的DNA计算出新僵尸的DNA。

僵尸最喜欢猎食什么物种呢？
等你学完第二课就知道了！

# 实战演习

右边是一个简单的猎食演示。点击一个“人”，看看僵尸猎食的时候会发生什么?
可见，新僵尸的DNA是通过从原来的僵尸的DNA, 加上猎物的DNA计算得来的。

学完这一章，请点击“下一章”， 我们该让游戏支持多玩家模式了。