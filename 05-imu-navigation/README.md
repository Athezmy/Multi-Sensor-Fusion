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


## gnss-ins-sim生成仿真数据

将ref_pos写入rosbag中，注意记录初始位姿，最后在odom中减去初始位姿：

<img src="imgs/4.11.png"> 
<img src="imgs/4.12.png"> 

记录gnss-ins-sim中静止状态重力矢量，解算程序中对应修改：

<img src="imgs/4.13.png"> 
<img src="imgs/4.14.png"> 

## 对比欧拉法和中值法精度差异与运动状态关系

### 静止状态

<img src="imgs/5.11.png">

euler：

<img src="imgs/5.12.png">
<img src="imgs/5.13.png">

mid-value：

<img src="imgs/5.14.png">
<img src="imgs/5.15.png">

### 匀速

<img src="imgs/5.20.png">
<img src="imgs/5.21.png">

euler:

<img src="imgs/5.22.png">

mid-value：

<img src="imgs/5.23.png">

### 匀加速

<img src="imgs/5.31.png">
<img src="imgs/5.32.png">

euler:

<img src="imgs/5.33.png">

mid-value：

<img src="imgs/5.34.png">


### 转弯

<img src="imgs/5.41.png">
<img src="imgs/5.42.png">

euler:

<img src="imgs/5.43.png">

mid-value：

<img src="imgs/5.44.png">

### 总结

可以看出静止状态和匀速状态下欧拉法和中值法差别很小  
匀加速状态中值法精度明显优于欧拉法  
在设定的多转弯状态下中值法精度也稍好于欧拉法  

解算过程中欧拉法取的是上一时刻状态，中值法对上一时刻和当前时刻状态做了平均。   
1、静止和匀速状态下没有速度变化，积分的值相同，两种解算结果应该一致；  
2、匀加速状态欧拉法积分结果小于中值法，匀减速状态欧拉法积分结果大于中值法，理论上中值法结果应该更加准确；  
3、在转弯较多情况下中值法对速度积分结果也应该更为准确。  














