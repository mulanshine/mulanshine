---
layout: post
title: "CNN-AlexNet"
date: 2018-04-19-20:37
categories: [卷积神经网络发展,论文]
tags: [论文,CNN,AlexNet]
---
# AlexNet

    - 分组卷积：将channels细分成多个group，再分组进行convolution。
    - 出现：论文：AlexNet, 卷积操作在两个GPU上进行。
    - 呈现结果：并行化计算，提升训练速度，输出的channel是 input channels / #groups
         （减小了参数，那是不是也reduce overfitting呀）
         
## 论文：

    ImageNet Classification with Deep Convolutional Neural Networks
    
## 作者：

    Alex Krizhevsky，Ilya Sutskever，Geoffrey E. Hinton
    
## 会议：

    NIPS 2012
    
## 成果：

    飞跃性进展，top-5: 18.9%
    
## 源起：

    硬件资源有限；计算量过大，分开计算；减小参数；
    
## 借鉴：

    Dropout、ReLU
    
## 理解：

    1)	ReLU:解决梯度饱和问题
    2)	GPU:两块并行加快计算
    3)	LRN:平滑处理
    4)	Overlapping Pooling:s<z
    5)	Dropout:reduce 过拟合
    
## 架构：

![AlexNet.png](https://github.com/mulanshine/mulanshine/raw/master/assets/pictures/AlexNet.png )
 
 具体细节见论文。
 
