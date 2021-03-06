---
title: "Deep Learning Notes"
date: 2018-07-10
draft: false
---

---
# 深度学习
## 模式识别：
- 计算机--记录计算  -> 人--感知理解信息   
- 通过计算机用数学技术方法来研究模式的自动处理和判别
- 模式：环境与个体
- 机器学习：machine  learning   利用计算机模拟实现人类学习行为，以获取新的知识和性能
- 模式识别过滤垃圾数据？--数据预处理？
- 识别基因序列的功能
- 股票预测--金融计算
## 模式识别方法：
### 句法模式识别
- 符号串，树，句法，分类  类似字典
- 首先提取基元，建立联系，文法规则判断分析
- 主要方法-自动机技术，
- 特点：分解的方法，干扰噪声导致抽取特征困难易失误
### 统计模式识别
-	特征向量，条件概率分布,维度高
-	主要方法-线性，非线性，数理统计，bayes决策，聚类分析
-	特点：成熟，
### 人工神经网络法
-	一种运算模型，大量节点相互连接构成
-	特点:太多参数难以训练
### 深度神经网络
-	很多层的神经网络，SVM-单层神经网络
-	特点：识别边缘特征
-	应用：物体识别
### 模式识别系统：
-	特征提取，特征选择，学习和训练，分类识别
-	分类正确率特征数
-	维数灾难：n维分成3^n，指数爆炸
-	把空间分成多个区域，哪个区域某个类别样本最多，分成过多格子，没有样本，无法估计识别
-	比较简单的模型会有更好的推广性
-	目标函数=训练误差+正则项
-	分类器形式，分类器参数
-	数据特征分布特性初步了解
-	评价：训练错误率很低但是验证错误率很高，过拟合
-	监督学习：已知分类
-	非监督学习：分类未知
## 数学基础：
### 基本定义：
-	transpose 转置   
-	概率P  0< P <1
-	概率密度函数p  p > 0
-	矩阵的性质：AB/=BA   AI=A  A（B+C）=AB+AC  乘法  特征值，方阵
-	导数：矩阵求导？matrix cookbook 
-	随机变量
-	方差，协方差，独立性。。。