---
classes: wide
title: "重心坐标空间及其应用-2020-10-14"
last_modified_at: 2020-10-14
excerpt: ""
categories:
  - other
tags:
  - math
  - 三角形
---

### 定义
三角形所在的平面上的任意点都能表示为3个顶点的加权值，  
这个权值就是**重心坐标**,从重心坐标$(b_1,b_2,b_3)$到标准3D空间的转换：  
$(b_1,b_2,b_3) \Longleftrightarrow b_1v_1+b_2v_2+b_3v_3$  
$b_1+b_2+b_3=1$  
$b_1,b_2,b_3$的值是每个顶点对该点的“贡献”   
不仅仅三角形内部，三角形平面上所有的点都能用重心坐标表示  
由三角形所确定的平面有2个自由度,三角形确定了一个子空间rank为2  


### 2D空间中的重心坐标
三个顶点 $p_1(x_1,y_1)$ &nbsp; $p_2(x_2,y_2)$ &nbsp; $p_3(x_3,y_3)$  
重心坐标 $b_1+b_2+b_3=1$  
2D坐标 $p(x,y)$  
矩阵形式$Ab=p$ :  

$$
\left(\begin{array}{ccc}
  x_1 & x_2 & x_3\\
  y_1 & y_2 & y_3\\
  1 & 1 & 1
\end{array}\right) \left(\begin{array}{c}
  b_1\\
  b_2\\
  b_3
\end{array}\right) = \left(\begin{array}{c}
  x\\
  y\\
  1
\end{array}\right)
$$

### 应用  
1.判断点在三角形内外，重心坐标有一个分量为负，在三角形外，否则在内  
2.两个三角形平面坐标映射  
给定两个三角形：  
三角形A $p_1(x_1,y_1)$ &nbsp; $p_2(x_2,y_2)$ &nbsp; $p_3(x_3,y_3)$ ,  
三角形B $p_4(x_4,y_4)$ &nbsp; $p_5(x_5,y_5)$ &nbsp; $p_6(x_6,y_6)$  
两个三角形三个顶点分别对应，A上一点$p_A$,求在B上对应的点$p_B$  

### $R^n$中的重心坐标
三角形确定的平面的rank为2，也就是能找到一组**正交基**$<a,b>$  
将该平面上的点，用新的坐标系表示，$R^n$坐标转化为$R^2$坐标  
这样就可以使用2D空间中重心坐标的处理方法  
