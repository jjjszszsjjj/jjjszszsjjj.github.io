---
title: course_wiki
date: 2022-05-01 21:52:06
tags:
 - basic
 - start
---

OpenFOAM Wiki的["3 weeks" series](https://wiki.openfoam.com/index.php?title=%223_weeks%22_series)

## Day One

### icoFoam 求解器
用于求解不可压缩牛顿流体的层流流动，基于PISO(pressure-implicit split-operator)算法:  
压力-速度迭代求解瞬态问题。每个迭代步中，利用一个预测步求解动量方程，再进行两步校正  
分别修正速度与压力。

### 关于网格  
当含有内部面时的操作`fluent3DMeshToFoam`,转换时内部面保持不变

### 软链接
由于之前运行过算例及不同网格, 建立软链接方式为:在软链接文件夹内($FOAM_RUN/day_1)
`ln -s /mnt/d/OFTutorialSeries/elbow/ basic_setup`

### 标准单位制

|质量|长度|时间|温度|摩尔数|电流|发光强度|
|:----:|:---:|:---:|:---:|:---:|:---:|:---:|
|kg|m|s|K|mol|a|c|
