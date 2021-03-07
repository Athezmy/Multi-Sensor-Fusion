# homework 6


## 完成中值法解算

按照TODO提示填空
<img src="imgs/1.1.png"> 

中值法结果如下：
<img src="imgs/1.2.png"> 

## 完成欧拉法解算
角度和速度变化函数有差别

<img src="imgs/2.1.png"> 
<img src="imgs/2.2.png"> 
<img src="imgs/2.3.png"> 

欧拉法解算结果如下：

<img src="imgs/2.5.png">

## 精度对比分析
更新位姿时保存解算位姿和ground_truth
<img src="imgs/3.01.png"> 
<img src="imgs/3.02.png"> 
<img src="imgs/3.03.png"> 

使用evo评测，欧拉法ape和轨迹如下：
<img src="imgs/3.11.png"> 
<img src="imgs/3.12.png"> 
<img src="imgs/3.13.png"> 
<img src="imgs/3.14.png"> 

中值法ape和轨迹如下：
<img src="imgs/3.21.png"> 
<img src="imgs/3.22.png"> 
<img src="imgs/3.23.png"> 
<img src="imgs/3.24.png"> 

可以看出在给定的数据下中值法精度要优于欧拉法。



