# homework4


## 1.跑通建图流程，保存地图并显示完整地图
<img src="img/1.png"> 

## 2.加载点云地图，在原点实现初始化
### 方式一：SetScanContextPose
<img src="img/2.1.png"> 
<img src="img/2.2-0s.png">

### 方式二：SetGNSSPose
<img src="img/3.1.png">
<img src="img/3.2原点.png">


## 3.全局初始化
### 方式一：SetScanContextPose
#### 首先记录初始位置gnss信息
<img src="img/2.3.png">

#### 计算和初始化位置的偏差并修正
<img src="img/2.4.png">

#### 100s初始化
<img src="img/2.5-100.png">
### 200s初始化
<img src="img/2.6-200.png">
### 300s初始化
<img src="img/2.7-300.png">
#### 400s初始化
<img src="img/2.8-400.png">

### 方式二：SetGNSSPose
<img src="img/3.3.png">

#### 100s初始化
<img src="img/3.4-100.png">
#### 200s初始化
<img src="img/3.5-200.png">
#### 300s初始化
<img src="img/3.6-300.png">
#### 400s初始化
<img src="img/3.7-400.png">





