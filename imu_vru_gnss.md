## IMU
`Inertial Measurement Unit` 中文译称“惯性测量单元”，包含`陀螺仪，加速度计。`IMU将所有运动视作直线运动与旋转运动的总和，因而通过 **加速度计测得直线运动，通过陀螺仪测得旋转运动**，进而和初始姿态相对比，得到当前的状态与相对位移，并不依赖外部的重力场或磁场，可以在任何情况下使用（精度够高的话）。

## AHRS
AHRS`（Attitude and Heading Reference System）`俗称航姿参考系统，AHRS由加速度计，磁场计，陀螺仪构成，能够为飞行器提供航向(yaw)，横滚(roll)和侧翻(pitch)信息
* AHRS比IMU增加了一个磁场传感器,通过磁场和重力场修正IMU


## VRU
#### IMU与VRU的区别
```
1. IMU只输出加速度传感器和陀螺仪的原始数据,没有欧拉角(横滚,俯仰)信号输出,而VRU则带有算法计算输出欧拉角信号
2. 
```

## GNSS
`Global Navigation Satellite System`全球导航卫星系统，包括GPS,GLONASS，北斗卫星导航系统 （BDS）


## INS
全称`Inertial Navigation System`即惯性导航系统。IMU是测量角速度和加速度的装置，**INS是通过测量得出的角速度和加速度的数值可以确定运动载体在惯性参考坐标中的运动**

型号|类型|接口|主要数据
|:--|:--|:--|:--
HWT101|IMU|TTL|角速度、航向（无参考）
WT31|IMU|TTL|加速度，横滚、俯仰角度
JY31N|IMU|TTL|加速度，横滚、俯仰角度
HWT31|IMU|TTL|加速度，横滚、俯仰角度
JY60|VRU|TTL|加速度，角速度，横滚、俯仰、航向（无参考）
JY61|VRU|TTL|加速度，角速度，横滚、俯仰、航向（无参考）
JY62|VRU|TTL|加速度，角速度，横滚、俯仰、航向（无参考）
JY61P|VRU|TTL|加速度，角速度，横滚、俯仰、航向（无参考）
JY901|AHRS+可接GPS|TTL|加速度，角速度，横滚、俯仰、航向（参考）、磁场
JY901S|AHRS+可接GPS|TTL|加速度，角速度，横滚、俯仰、航向（参考）、磁场
JY901B|AHRS+可接GPS+气压|TTL|加速度，角速度，横滚、俯仰、航向（参考）、磁场、气压
JY931|AHRS|TTL|加速度，角速度，横滚、俯仰、航向（参考）、磁场
