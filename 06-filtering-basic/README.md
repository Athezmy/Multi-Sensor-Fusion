# homework 6

## 1.补全滤波代码

修改F矩阵和B矩阵，对应公式填写代码

<img src="images/1.1.png"> 
<img src="images/1.3.png"> 
<img src="images/1.4.png"> 
<img src="images/1.5.png"> 
<img src="images/1.6.png"> 

滤波结果如下：

<img src="images/1.7.png"> 

## 2.调试参数，使得滤波后性能更好

初始参数evo评测结果如下：

<img src="images/2.11.png"> 
<img src="images/2.12.png"> 
<img src="images/2.13.png">

分别增大和减小先验噪声P

<img src="images/2.21.png"> 
<img src="images/2.22.png"> 
<img src="images/2.23.png">

<img src="images/2.31.png"> 
<img src="images/2.32.png"> 
<img src="images/2.33.png">

增大过程噪声Q，减小测量噪声R

<img src="images/2.41.png"> 
<img src="images/2.42.png"> 
<img src="images/2.43.png">

减小过程噪声Q，增大测量噪声R

<img src="images/2.51.png"> 
<img src="images/2.52.png"> 
<img src="images/2.53.png">

分析发现：  
P 是误差协方差初始值，表示对当前预测状态的信任程度    
Q越大越信任观测值  ，融合结果和激光更接近  
R越大越信任预测值

调出的一组较优参数如下：

<img src="images/2.61.png"> 
<img src="images/2.63.png"> 
<img src="images/2.62.png">

融合后evo评测ape的结果中 max、mean、median、min都是融合后更优，其他参数也更为接近

## 3.不考虑随机游走推导模型并实现，对比性能差异并给出对比结果

主要是B矩阵形式不同

<img src="images/3.3.jpg">
<img src="images/3.1.png"> 
<img src="images/3.2.png"> 

设置了与2中相同的6组参数：

<img src="images/4.11.png"> 
<img src="images/4.12.png"> 
<img src="images/4.13.png">

<img src="images/4.21.png"> 
<img src="images/4.22.png"> 
<img src="images/4.23.png">

<img src="images/4.31.png"> 
<img src="images/4.32.png"> 
<img src="images/4.33.png">

<img src="images/4.41.png"> 
<img src="images/4.42.png"> 
<img src="images/4.43.png">

<img src="images/4.51.png"> 
<img src="images/4.52.png"> 
<img src="images/4.53.png">

<img src="images/4.61.png"> 
<img src="images/4.62.png"> 
<img src="images/4.63.png">





