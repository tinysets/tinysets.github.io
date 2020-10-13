---
classes: wide
title: "重心坐标空间及其应用-2020-10-13"
last_modified_at: 2020-10-13
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
$b_1,b_2,b_3$的值是每个顶点对该店的“贡献”   
不仅仅三角形内部，三角形平面上所有的点都能用重心坐标表示

### 2D中的三角形
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