---
title: "Deep Learning Notes"
date: 2018-07-24
draft: false
---

---
# 计算机视觉与深度学习
## 概率论相关概念
- 伯努利分布 零一分布，两点分布
- 二项分布  n次独立的伯努利试验
- sigmoid函数  s(x)=1/(1+e^-x)  单调递增  值域=[0，1] 神经网络的阈值函数
- 高斯分布  正态分布   高斯函数   中心极限定理  N维正态分布
- 信息论  信息量I(x)=-logP(x)  概率越小信息量越大  熵H(x)=IEx~P[I(x)]  信息量的数学期望   KL衡量分布间的差异
- 多变量正态分布  均值决定中心点  方差决定联展程度  协方差矩阵，如果xi与xj相互独立，则非对角线的元素都是0
- 马氏距离
- 高斯变量的线性变换仍然服从高斯分布  把协方差变成单位阵
## 分类
- 两类情况  贝叶斯定理？
- 参数估计  最大似然估计  原理-概率大的更可能发生
- 贝叶斯参数估计  随机变量  参数的先验分布  后验概率密度