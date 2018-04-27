---
title: 基于深度学习和卷积神经网络的快速风格迁移
date: 2017-12-30 19:58:53
tags: 
- 深度学习
- 卷积神经网络
---

之前使用了谷歌深度学习的开源神器`Deeplearn.js`，利用这个深度学习框架，也根据Official Demo实现了前端的快速风格迁移。

使用这个库在前端风格迁移的主要流程就是读取`Tensorflow`训练出的`checkpoints`作为模型输入参数，然后在依赖`Canvas`和`WebGL`接口进行计算和渲染。速度比原来2015年的论文[A Neural Algorithm of Artistic Style](https://arxiv.org/abs/1508.06576)在Github的实现快了许多，但是作为代价，训练风格模型需要更加的耗时。

<!-- more -->

## Style 图片选择

我选择了今年暑假在兽夏祭上抢到的《世界之旅》中蝴蝶谷的插画：

**蝴蝶谷 Monarch Butterfly Biosphere Reserve**

插画的作者是[`薄荷犬Enma`](http://enmah.lofter.com/)

![btfly](/images/fast-style-transfer/btfly.jpg)

## 为什么选择这张图？

~~我爱夏泽尔~~

因为这张图细节纹理良好，如图：

![detail](/images/fast-style-transfer/texture.png)

主要是蝴蝶的边缘纹理比较清晰，而且黄昏时的地面上也有**足够多的细节**。实际上，提取风格的并不会指的是夏泽尔本人，而是夏泽尔、草地、蝴蝶的一种深层次“抽象”。

这是因为，在卷积神经网络后的最底层，已经看不清楚夏泽尔是夏泽尔了，剩下的是夏泽尔的一种“特征”的体现。但是实际上，夏泽尔占整幅图的比重很小，所以大多是提取到蝴蝶和草地的深层次特征。

## 过程

环境：

- 操作系统：Windows 10
- 显卡： NVD GTX 1060 6GB
- cuDnn: 6.x
- cuda: 8.x
- Tensorflow: 1.3

实际上大概跑了8个小时，训练集是`train2014`，每次`Epoch`迭代1000次，`batch size`为6。

## 结果

- 城市

![case01](/images/fast-style-transfer/case01.png)

输出：

![city](/images/fast-style-transfer/output-city.jpg)

- 台北101

![tai101](/images/fast-style-transfer/case02.png)

输出：

![101](/images/fast-style-transfer/output-101.jpg)

- 花村 - 守望先锋

![huacun](/images/fast-style-transfer/case03.png)

输出：

![huacun](/images/fast-style-transfer/output-huacun.jpg)

## 总结

怎么样，很酷吧。