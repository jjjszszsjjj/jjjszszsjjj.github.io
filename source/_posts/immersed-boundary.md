---
title: I Want to Be Strong
comments: true
date: 2022-05-14 15:39:33
tags: 
categories:
---
### Ghost-Cell IBM 
[cfd-online arjun](https://www.cfd-online.com/Forums/main/94956-how-find-ghost-cells-immersed-boundary-methods.html)
![](/images/immersed-boundary/f1.png "原始方程求解")
力源项施加到流体相动量方程，而固体相内部网格速度等于颗粒速度。而压力由连续性方程求解得到包含流体、固体域整体的结果

![](/images/immersed-boundary/f2.png "动量方程修正")
通过修改ghost-cell值使原求解形式中梯度（扩散项）等变量在被边界截断时可以为实际情况。

![](/images/immersed-boundary/f3.png "方法核心")
遍历全部网格,对于流体网格,当其邻居中具有在颗粒内部的网格时便是ghost-cell，进而修改上述ghost-cell值。
而在整个区域内标记solid具有不同的方法,该作者未予以公开。

![](/images/immersed-boundary/f4.png "固体区域网格识别")
固体区域识别算法:采用三维遍历或最近邻搜索