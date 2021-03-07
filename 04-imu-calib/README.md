# homework 5


## 完成雅克比推导

公式符号与代码中形式保持一致
<img src="img/1.1.jpg"> 
<img src="img/1.2.jpg"> 

## 完成新的内参模型下的标定
根据TODO提示改成下三角

<img src="img/2.1.png"> 
<img src="img/2.2.png"> 
<img src="img/2.3.png"> 

残差改为ppt中平方的形式

<img src="img/2.4.png">

标定结果如下：
<img src="img/2.5.png"> 

##  使用解析式求导完成标定
构建ceres求解器:
<img src="img/3.1.png"> 

CostFunction:
<img src="img/3.2.png"> 

雅克比：
<img src="img/3.3.png"> 
<img src="img/3.4.png"> 

标定结果与自动求导结果一致
<img src="img/3.5.png"> 

