# homework9

## 1.推导雅各比，补全代码

雅各比推导如下：

<img src="imgs/1.1.jpg"> 

imu预积分状态更新如下：

<img src="imgs/1.2.png"> 

更新F和G矩阵：

<img src="imgs/1.3.png"> 

g2o计算误差：

<img src="imgs/1.4.png">

加法运算定义如下：

<img src="imgs/1.5.png">

运行结果：

<img src="imgs/1.6.png"> 

## 2.实现和不加IMU时的效果对比分析

没有IMU预积分ape:

<img src="imgs/2.1.png">

有IMU预积分ape:

<img src="imgs/2.2.png">

可以看出有IMU预积分后误差最大值和标准差都有改善。

无IMU预积分部分地图：

<img src="imgs/2.3.png"> 

添加IMU预积分部分地图：

<img src="imgs/2.4.png">

通过对比可以发现增加IMU预积分后地图细节更加完善。

## 3.融合编码器预积分推导

<img src="imgs/3.1.jpg"> 

<img src="imgs/3.2.jpg"> 

<img src="imgs/3.3.jpg"> 


