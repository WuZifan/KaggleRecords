# KaggleRecords
Record my kaggle experiences.

## 1. [House Pricing](https://github.com/WuZifan/KaggleRecords/tree/master/House%20Prices)

问题描述：

 1、给出某地区房子的一些特征以及价格。
 2、特征中包括numerical特征和category特征。
 3、所需要预测的量为连续性特征（numerical），即是一个回归问题。

### 1.1 [第一次尝试](https://github.com/WuZifan/KaggleRecords/blob/master/House%20Prices/House_Pricing.ipynb)

采用模型：

 1、最基本的线性模型。
 2、Lasso（L1正则化）
 2、Ridge（L2正则化）

模型融合策略：

 对三者结果取均值。

### 1.2 [第二次尝试](https://github.com/WuZifan/KaggleRecords/blob/master/House%20Prices/House_Pricing2.ipynb)

采用模型：

 1、基本的线性模型
 2、Lasso+CV寻找最优参数
 3、Ridge+CV寻找最优参数

模型融合策略：

 1、基本线性模型严重过拟合，抛弃。
 2、对剩下的两个采用取均值策略。

### 1.3 [第三次尝试](https://github.com/WuZifan/KaggleRecords/blob/master/House%20Prices/House_Pricing3.ipynb)

采用模型：

 1、xgboost的回归版本
 2、randomforest的回归版本
 3、adaboost的回归版本
 4、bagging的回归版本
 
模型融合策略：

 1、对四者取均值
 
## 2. [Titanic](https://github.com/WuZifan/KaggleRecords/tree/master/Titanic)

问题描述：

 1、给出部分泰坦尼克号上的乘客的特征与获救情况。
 2、特征中有category和numerical值，且总共只有7个特征。
 3、预测剩下的乘客哪些存活，哪些死亡，是一个分类问题。

### 2.1 [第一次尝试](https://github.com/WuZifan/KaggleRecords/blob/master/Titanic/Titanic1.ipynb)

采用模型：
 
 logistics回归+cv

### 2.2 [第二次尝试](https://github.com/WuZifan/KaggleRecords/blob/master/Titanic/Titanic2.ipynb)
 
采用模型：

 1、logistic+cv
 2、svm+cv
 3、randomforest+cv

模型融合：

 简单的voting。

## 3. [Digital Recognize](https://github.com/WuZifan/KaggleRecords/tree/master/DigitRecognizer)

### 3.1 [第一次尝试](https://github.com/WuZifan/KaggleRecords/blob/master/DigitRecognizer/Digital_Recognize1.ipynb)

采用模型：

 简单的ANN
 1. 激活函数：softmax
 2. 损失函数：交叉熵
 3. 优化方式：梯度下降
 4. 输入层：784个节点，对应每个像素点。
 5. 隐层：只有一个隐层，10个节点，同时作为输出层。
 6. 输出层：就是隐层。
 
 ### 3.2 [第二次尝试](https://github.com/WuZifan/KaggleRecords/blob/master/DigitRecognizer/Digital_Recognize2.ipynb)
 
 采用模型：
 
  3层CNN。（ tensorflow)
 
 ### 3.3 [第三次尝试](https://github.com/WuZifan/KaggleRecords/blob/master/DigitRecognizer/Digital_Recognize3.ipynb)
 
 采用模型：
 
  多层CNN。（keras）
  
 
