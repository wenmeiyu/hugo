---
title: "Data Mining Notes-neural network"
date: 2018-07-12
draft: false
---

---
- 多模型集成
- 偏置项？转递函数？权重-向前向后学习的结果
- 向前学习：计算每个节点的影响  一个网络结构  初始化设置的权重
- 向后学习backpropagation：求解  梯度下降法求导  目标求导的过程
- 不断和实际值比较，获得最佳残差
- 目标函数=损失函数？
- 一步一步逼近最优解
chain rule  劣势规则？  practice  求导
## 激活函数：  一般神经元上选择非线性函数-
-	sigmoid：它的求导简单  结果映射到01之间，可以表示成概率  最后一层常用  针对二分类问题
-	tanh： cnn 和 lstm常用  出最后一层之外  映射到-1到1之间，使均值为0
-	ReLU Rectified Linear Unit:收敛更快  网络很深时，例如cnn  文本领域很少使用，信息不规整，信息更复杂
-	改进的ReLU：Leaky ReLU
-	Softmax： 一般不在中间层用  最后一层常用   针对多分类问题
- batch_size：更新参数，算完部分例子之后更新
- 凸优化问题-可以得到全局最优解  
---
# 优化模型，提高算法，解决过拟合问题，学习率的设置，权值初始化
- 深度神经网络的三步：向前学习，向后学习，权值更新
- SGD Stochastic  gradient  descent  随机梯度下降：更快的收敛，加速BSD？一个一个样例计算  is often  better 防止过拟合
- Mini-batch Gradient Descent 
- 归一化 ：
- 防止过拟合的方法：
- 	batch normalization：
- 	L1-regularization 可以做特征选择   L2-regularization
- 	Early  stopping  早期结束  当连续两三次epoch不变时暂停
- 	Dropout ：每次选择性地抛弃一些神经元  防止过拟合，主要应用于深度学习  没有理论验证  调参每一层抛弃多少神经元
- 学习率，学习率下降到最后会震荡，
## 降低学习率的方法：
- Adagrad：自适应
- RMSprop  :
- Adadelta  :
- Adam:
- AdaSecant:
