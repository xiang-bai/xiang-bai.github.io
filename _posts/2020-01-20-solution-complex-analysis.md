---
layout: post
title:  "复变函数基础习题解答"
date:   2020-01-20 02:34:20 +0800
categories: math
tags: analysis
---

# 复变函数基础习题解答

## 简介

文章是<a href="complex-analysis">复变函数基础</a>中习题的解答。

## 第一章 复数及复平面

1. 试用复数表示圆方程
 $$a(x^2+y^2)+bx+cy+d=0,$$
 其中，$a,b,c,d$是实常数（如果$a=0$，$b,c$不全为$0$，这时方程为直线方程）。
 **解**. 设$z=x+iy$，则有$x^2+y^2=z\bar{z}$，$x=\frac{z+\bar{z}}{2}$，$y=\frac{z-\bar{z}}{2 i}$，带入方程有
 $$a(z\bar{z})+\beta z+\bar{\beta}\bar{z}+d=0,$$
 其中，$\beta=\frac{b-ic}{2}$.
2. 设$z_1,z_2$为两个复数，则
 $$\overline{z_1+z_2}=\bar{z_1}+\bar{z_2},\ \ \overline{z_1 z_2}=\bar{z_1}\bar{z_2},\ \ \overline{\overline{z_1}}=z_1.$$
 对于乘法有
 $$|z_1z_2|=|z_1||z_2|,\ \ \text{Arg }(z_1z_2)=\text{Arg }z_1+\text{Arg }z_2.$$
 对于除法有，
 $$|\frac{z_1}{z_2}|=\frac{|z_1|}{z_2},\ \ \text{Arg }\frac{z_1}{z_2}=\text{Arg }z_1-\text{Arg }z_2.$$
3. 设$z_1,z_2$是两个复数，证明
 $$|z_1+z_2|^2=|z_1|^2+|z_2|^2+2\Re{(z_1 \bar{z_2)}},$$
 并且
 $$|z_1+z_2|\le |z_1|+|z_2|.$$

4. 做复平面$\mathbb{C}$上不同两点$a,b$的直线和不同不共线三点$a,b,c$的圆的表达式。
5. 求$\sqrt[4]{1+i}$的所有值。
6. 集合$\{z\mid (1-i)z+(1+i)\bar{z}>0\}$是一半平面，是一个单连通无界区域，边界为直线$(1-i)z+(1+i)\bar{z}=0$，即$x+y=0$。
7. 集合$\{z\mid 2<\Re{z}<3\}$为一垂直带形，它是单连通无界区域，其边界为直线$\Re{z}=2$和$\Re{z}=3$。
8. 集合$\{z\mid 2<\arg{z-i}<3\}$为一角形，它是单连通无界区域，其边界为半射线$\arg{z-i}=2$和$\arg{z-i}=3$。
9. 集合$\{z\mid 2<\vert{z-i}\vert<3\}$为一角形，它是多连通有界区域，其边界为圆$\vert{z-i}\vert=2$和$\vert{z-i}\vert=3$。
10. 在$\mathbb{C}_ {\infty}$，集合$\{ z\mid 2 < \vert z\vert \le + \infty \}$和$\{ z\mid 2< \vert z\vert< +\infty \}$分别是单连通和多连通的无界区域，边界分别是$\{z\mid \vert z\vert=2\}$和$\{z\mid \vert z\vert=2\}\cup \{\infty\}$。



## 第二章 复变函数

1. 复变函数$f(z)=z^2=(x^2-y^2)+2ixy$和$f(z)=\mathrm{e}^{x}\cos{y}+i\mathrm{e}^{x}\sin{y}$在复平面上解析。

1. 复变函数$f(z)=\bar{z}=x-iy$在任何点都不可微。

1. 作出一个含$i$的区域，使得函数
 $$w=\sqrt{z(z-1)(z-2)}$$
 在区域内可分解成解析分枝，求一个分枝在$i$的值。

1. 验证函数$w=\sqrt[4]{z(1-z)}$在区域$D=\mathbb{C}-[0,1]$可以分解成解析分枝，求出函数在$(0,1)$上沿正实值的一个分枝在$z=-1$处的值，以及函数在$(0,1)$下沿的值。

## 第三章 复变函数的积分

1. 设$C$是连接$z_0$和$Z$的简单曲线，则
 $$\int_{C}\mathrm{d}z=Z-z_0,$$
 $$\int_{C}z\mathrm{d}z=\frac{1}{2}(Z^2-z_0^2).$$
 **解**：将$f(z)=1$和$f(z)=z$带入积分定义容易得到。

2. 设$C$是圆$\vert z-\alpha\vert =\rho$，其中$\alpha$是一复数，$\rho$是正数，则按逆时针方向所取的积分是
 $$\int_{C}\frac{\mathrm{d}z}{z-\alpha}=2\pi i.$$
 **解**：设$z-\alpha=\rho \mathrm{e}^{i\theta}$，则$\mathrm{d}z=\rho i\mathrm{e}^{i\theta}\mathrm{d}\theta$，因此
 $$\int_{C}\frac{\mathrm{d}z}{z-\alpha}=\int_{0}^{2\pi}i\mathrm{d}\theta=2\pi i.$$

1. 设$D$是不包含$\alpha$的单连通区域，并且$z_0,z\in D$，则
  $$\int_{z_0}^{z}\frac{\mathrm{d}\zeta}{(\zeta-\alpha)^m}=\frac{1}{1-m}\Big{(}\frac{1}{(z-\alpha)^{m-1}}-\frac{1}{(z_0-\alpha)^{m-1}}\Big{)}$$
  其中，$m$是不为$1$的整数。另外，设$D$在复平面上沿从$\alpha$出发的任何射线而割开的区域内，则
  $$\int_{z_0}^{z}\frac{\mathrm{d}\zeta}{\zeta-\alpha}=\ln {(z-\alpha)}-\ln{(z_0-\alpha)},$$
  其中对数是$\mathrm{Ln}(z-\alpha)$在$D$内的一个解析分枝在$z,z_0$的值。

2. 在圆环$D:R_1<\vert z\vert<R_2(0<R_1<R_2<+\infty)$内，$f(z)=\frac{1}{z}$解析。取两点$z_0,z_1\in D$，做两条连接$z_0,z_1$的曲线$C_1$和$C_2$如图![Alt text](./pic3.17.png)。取定$\mathrm{Arg }z$在$z_0$处的值是$\arg {z_0}$，当$z$沿$C_1$从$z_0$连续运动到$z_1$时，$z$的辐角从$\arg{z_0}$变化到$\arg{z_1}$，当$z$沿$C_2$从$z_0$连续运动到$z_1$时，$z$的辐角从$\arg{z_0}$变化到$\arg{z_1}-2\pi$。求$\frac{1}{\zeta}$沿$C_1$的积分。
