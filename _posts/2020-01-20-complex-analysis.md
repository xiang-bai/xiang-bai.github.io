---
layout: post
title:  "复变函数基础"
date:   2020-01-20 02:34:20 +0800
categories: math
tags: analysis
---


# 复变函数基础

* any list
{:toc}

## 介绍

文章是学习复变函数的笔记，参考余家荣的复变函数。

## 第一章 复数及复平面

*目标：*
本章主要介绍复数及复平面的一些基本概念，包括复数的几何表示，区域和曲线等内容。通过本章教学，使学生熟练掌握复数的模和辐角、复数的三种表示方法、复数的基本性质，掌握复数的乘幂与方根的求法，会用复数表示平面图形；理解无穷远点、扩充复平面、复球面、区域、单连通区域、多连通区域、约当曲线、光滑（逐段光滑）曲线等概念。

*内容：*
- **复数**：每个复数$z$表示为$x+yi$，其中$x,y\in \mathbb{R}$，$i$为虚数单位(即$i^2=-1$，故也记作$\sqrt{-1}$).
- **实部和虚部**：对于复数$z=x+yi$，$x,y$分别称为$z$的实部和虚部，记作$x=\Re{z} $和$y=\Im{z}$
- **复平面**：由于$z=x+yi \to (x,y)$是$\mathbb{C}$到$\mathbb{R}^2$的双射，故称平面$\mathbb{R}^2$为复平面$\mathbb{C}$，每个点$(x,y)$称为$z=x+yi$。
- **复数向量表示**：复数$z=x+yi$可以视作实轴和虚轴投影为$x$和$y$的任意向量。
- **复数的模**：把向量$z=x+yi$的长度称为$z$的模，记作$\vert z\vert$。显然$\vert z\vert=\sqrt{x^2+y^2}=\sqrt{z\bar{z}}$。
- **辐角和主值**：向量$z$与实轴的夹角称为$z$的辐角，记作$\theta$。显然$\theta$有无穷多个值，记作$\text{Arg }{z}=\theta +2k\pi$($k\in \mathbb{Z}$)。$\text{Arg }{z}$中只有一个值$\alpha$满足$-\pi < \alpha \le \pi$，叫做$z$的主值记作$\arg{z}$。
- **复数三角表示**：复数$z=x+yi$可以通过辐角来表示，即$z=\vert z\vert(\cos{\text{Arg }z}+i\sin{\text{Arg } z})$.
- **共轭**：复数$z=x+iy$的共轭为$x-iy$，记作$\bar{z}$。显然$\text{Arg }z=-\text{Arg }z$.
- **乘幂**：设复数$z\neq 0$和正整数$n$，有
 $$z^{n}=\vert z\vert^n\Big{(}\cos(n\text{Arg }z)+i\sin(n\text{Arg } z)\Big{)}$$
 显然上式中$n=0$，$z^0=1$也成立。对于负数，$z^{-n}=\frac{1}{z^n}$，故
 $$z^{-n}=\vert z\vert^{-n}\Big{(}\cos(-n\text{Arg }z)+i\sin(-n\text{Arg } z)\Big{)}$$
 在上面做变量替换$z=w^n$，有
 $$z^{\frac{1}{n}}=\vert z\vert^{\frac{1}{n}}\Big{(}\cos(\frac{1}{n}\text{Arg }z)+i\sin(\frac{1}{n}\text{Arg } z)\Big{)}$$
- **De Moivre(棣莫弗)公式**：
 $$(\cos \theta +i\sin \theta)^n=\cos n\theta+i\sin n\theta.$$
- **球极**：在三维空间，把$xOy$平面看作$z=z+iy$平面，考虑球面$S$
 $$x^2+y^2+u^2=1,$$
 取定点$N(0,0,1)$称为球极。
- **球极映射**：对于$xOy$平面上一点$A(x,y,0)$，连接球极$N$与$A$的直线与球面的交点为$A'(x',y',u')$，称$A'$为$A$的球极映射。
- **无穷远点**：约定复平面上有一个理想点，它的球极映射为$N$，称为无穷远点，记作$\infty$，它的模约定为$+\infty$.
- **扩充复平面**：复平面$\mathbb{C}$与无穷远点组成的集合称为扩充复平面$\mathbb{C}_ {\infty}$，记作$\mathbb{C}_ {\infty}=\mathbb{C}\cup \{\infty\}$.
- **复球面**：上述几条在球面$S$与扩充复平面$\mathbb{C}_ {\infty}$上建立了双射，这种球面称为复球面。
- **区域**：如果复平面$\mathbb{C}$上的点集$D$满足
 (a). $D$为开集；
 (b). $D$满足连通性，即$D$中任意两个有限点，可以用有限个连接的线段构成的折线连接起来，并且折线上的点全部属于$D$；
 则称$D$为区域。如果$z(a)=z(b)$，称为约当闭曲线。
- **约当曲线**：设$z=z(t)(a\le t\le b)$的实部和虚部在$[a,b]$上都关于$t$连续，则集合$\{z(t)\vert t\in[a,b]\}$称为一条连续曲线。此外，如果不同两点$t_1,t_2\in[a,b]\big{(}(t_1,t_2)\neq (a,b)\big{)}$满足$z(t_1)\neq z(t_2)$，那么称$z=z(t)(a\le t\le b)$为简单连续曲线，或者约当曲线。
- **内区域与外区域**：任何一条约当闭曲线将整个平面分成两个区域，有界的一个称为内区域，无界的称为外区域。
- **光滑（逐段光滑）曲线**：对于连续曲线$z=z(t)(a\le t\le b)$，如果它的实部和虚部有连续导数，并且$z'(t)\neq 0$，则称为光滑曲线。通过有限条光滑曲线连接成的曲线称为逐段光滑曲线。
- **单连通区域和多连通区域**：设$D$为复平面$\mathbb{C}$上的区域，如果$D$内任何简单闭曲线的内区域中每一点都属于$D$，那么$D$称为单连通区域。不是单连通的区域称为多连通区域。对于$\mathbb{C}_ {\infty}$，单连通区域要求简单闭曲线的内区域或外区域的每个点都属于$D$.



## 第二章 复变函数

*目标：*
解析函数是本课程的主要研究内容。本章主要讲解复变函数、解析函数以及初等函数等内容。理解并掌握复变函数极限与连续性的概念与性质；理解解析函数的概念，理解函数在一点解析与函数在一点可微的区别，熟练掌握利用柯西-黎曼条件判别解析函数的方法；掌握指数函数、三角函数的定义和性质，注意与实指数函数、实三角函数的区别；理解对数函数、幂函数、反三角函数等初等多值函数产生多值的原因，并能掌握简单的初等多值函数分出单值解析分支的方法。

*内容：*
- **复变函数**：设复平面$\mathbb{C}$上给定点集$E$，如果又一个法则$f$，使得任意$z=x+iy\in E$，存在$w=u+iv\in \mathbb{C}$与之对应，则称$f$为$E$上的复变函数，记作$w=f(z)$。
- **极限**：假设$w=f(z)$定义在$E$上，$z_0$为$E$上的聚点，$\alpha$是复常数。如果对于任意的$\epsilon >0$，存在一个正整数$\delta >0$，满足当$z\in E$且$0<\vert z\vert <\delta$时有
 $$\vert f(z)-\alpha\vert <\epsilon,$$
 则称$\alpha$是$f(z)$在$z\to z_0$处的极限。
- **连续**：设函数$f(z)$定义在$E$上，并且$z_0\in E$，如果
 $$\lim\limits_{z\to z_0,z\in E}f(z)=f(z_0),$$
 则称$f(z)$在$z_0$处连续。如果$f(z)$在$E$上每一点都连续，则称$f(z)$在$E$上连续。
- **导数**：对于任意的$\epsilon>0$，存在$\delta >0$，满足当$z\in E$且$0<\vert z\vert <\delta$时有，
 $$\Big{\vert} \frac{f(z)-f(z_0)}{z-z_0}-\alpha \Big{\vert}<\epsilon,$$
 则称$f(z)$在$z_0$处可导，或者有导数$\alpha$，记作$f'(z_0)=\alpha$。
- **解析函数**：如果函数$f(z)$在区域$D$内每一点都可微，则称$f(z)$在区域$D$内解析。如果$f(z)$在$z_0$一个邻域内解析，则称$f(z)$在$z_0$点解析。
- **Cauchy-Riemann条件**：设$f(z)=u(x,y)+iv(x,y)$定义在区域$D$内，条件
 $$\frac{\partial u}{\partial x}=\frac{\partial v}{\partial y},\ \frac{\partial u}{\partial y}=-\frac{\partial v}{\partial x}$$
 称为Cauchy-Riemann条件。
 - **定理**：设$f(z)=u(x,y)+iv(x,y)$定义在区域$D$上，那么$f(z)$在$z=x+iy\in D$处可微的充分必要条件是在$z=x+iy$处，$u(x,y)$和$v(x,y)$都可微，并且满足Cauchy-Riemann条件。
 - **定理**：设$f(z)=u(x,y)+iv(x,y)$定义在区域$D$上，那么$f(z)$在$D$内可微的充分必要条件是在$D$内，$u(x,y)$和$v(x,y)$都可微，并且满足Cauchy-Riemann条件。
 - **推论**：当$f(z)$有导数的情况下，有
  $$f'(z)=\frac{\partial u}{\partial x}+i\frac{\partial v}{\partial x}=\frac{\partial v}{\partial y}-i\frac{\partial u}{\partial y}.$$
- **指数函数**：$\mathrm{e}^z=\mathrm{e}^x(\cos{y}+i\sin{y}).$
- **对数函数**：给定复数$z$，满足$z=\mathrm{e}^w$的复数$w$称为$z$的对数，记作$\mathrm{Ln}{z}$。其实，
 $$\mathrm{Ln}{z}=\ln{\vert z\vert}+i\mathrm{Arg}{z}.$$
 把$\ln{\vert z\vert}+i\arg{z}$定义为$\mathrm{Ln}{z}$的主值，记作$\ln z$。
- **幂函数**：设$\alpha$是复数，则复数$z$的$\alpha$次幂定义为
 $$z^{\alpha}=\mathrm{e}^{\alpha\mathrm{Ln}{z}}.$$
- **幂函数枝点**：
 - 对于有理数$\alpha=\frac{m}{n}$(既约分数)，称$0$和无穷远点$\infty$为$z^{\alpha}$的$n-1$阶枝点。
 - $\alpha$不是有理数时，原点和无穷远点是$z^{\alpha}$的无穷阶枝点。

- **三角函数**：正弦函数和余弦函数，
 $$\cos{z}=\frac{\mathrm{e}^{iz}+\mathrm{e}^{-iz}}{2},\ \ \sin{z}=\frac{\mathrm{e}^{iz}-\mathrm{e}^{-iz}}{2i}.$$
 反三角函数，
 $$\mathrm{Arc}\tan{z}=\frac{1}{2i}\big{(}\mathrm{Ln}(z-i)-\mathrm{Ln}(z+i)+i\pi\big{)}.$$


## 第三章 复变函数的积分 

*目标：*
本章主要介绍复积分的定义和性质，柯西积分定理、柯西积分公式、高阶导数公式、柯西不等式与刘维尔定理等内容。理解复积分的概念、性质，掌握复积分的计算方法；理解柯西积分定理，熟练掌握利用柯西积分定理计算函数沿闭曲线的积分；理解柯西积分定理的推广；理解柯西积分公式、高阶导数公式，熟练掌握利用柯西积分公式、高阶导数公式计算函数沿闭曲线的积分；了解解析函数的无穷可微性；了解柯西不等式与刘维尔定理，掌握其证明方法；掌握利用摩勒拉定理判断解析函数的方法。

*内容：*
- **复积分**：设$C$是简单(简单光滑或者简单分段光滑)曲线，复函数$f(z)$沿曲线$C$的积分$\int_{C}f(z)\mathrm{d}z$为
 $$\int_{C}f(z)\mathrm{d}z=\int_{C}u(x,y)\mathrm{d}x-\int_{C}v(x,y)\mathrm{d}y+i\Big{(}\int_{C}v(x,y)\mathrm{d}x+\int_{C}u(x,y)\mathrm{d}y\Big{)}.$$
 - 如果$C$是简单光滑曲线$z(t)(t_0\le t\le T)$，则有
 $$\int_{C}f(z)\mathrm{d}z=\int_{t_0}^{T}f(z(t))z'(t)\mathrm{d}t.$$
 - 如果在$C$上，$\vert f(z)\vert \le M$，且$C$的长度是$L$则$\big{\vert} \int_{C}f(z)\mathrm{d}z\big{\vert}\le ML$。

- **引理1**：设$f(z)$是单连通区域$D$内的解析函数，$C$是$D$内多边形的边界，则沿$C$的逆时针积分有
 $$\int_{C}f(z)\mathrm{d}z=0.$$   
 **证明**：先证三角形类似闭区间套定理构造嵌套三角形利用可微性使得积分值可以任意小，再把多边形分割为三角形。$\blacksquare$
- **不定积分**：设函数$f(z)$和$\Phi(z)$定义在区域$D$内，$\Phi(z)$是$D$上解析函数，并且有$\Phi'(z)=f(z)$，则称$\Phi(z)$为$f(z)$在$D$上的不定积分或者原函数。
- **凸区域**：对于区域$D$，如果任意$a,b\in D$，满足对于任意$0\le t\le 1$有$(1-t)a+tb\in D$，则称$D$是凸区域。
- **引理2**：设$f(z)$在凸区域$D$内解析，那么$f(z)$在$D$内有原函数。   
 **证明**：$\blacksquare$
- **引理3**：设$f(z)$在区域$D$内连续且有原函数$F(z)$，如果$a,b\in D$且$C$是连接$a$和$b$的曲线，那么
 $$\int_{C}f(z)\mathrm{d}z=F(b)-F(a).$$   
 **证明**：$\blacksquare$
- **Cauchy积分定理**：是$f(z)$是单连通区域$D$内的解析函数，则  
 (1). 设$C$是$D$内任一条简单闭曲线，那么
 $$\int_{C}f(z)\mathrm{d}z=0.$$
 其中，积分沿$C$的逆时针（或者顺时针）方向。
 (2). 设$C$是$D$内连接$z_0$和$z$的任一条简单曲线，那么沿$C$从$z_0$到$z$的积分只由$z_0$和$z$确定，与$C$无关，故积分记作$\int_{z_0}^{z}f(\zeta)\mathrm{d}\zeta$。   
 **(1)的等价刻画**：设$C$是一条简单闭曲线，函数$f(z)$在以$C$为边界的有界闭区域上解析，那么
 $$\int_{C}f(z)\mathrm{d}z=0.$$   
 **引理2推广**：设$f(z)$是单连通区域$D$内的解析函数，那么$f(z)$在$D$内有原函数。
- **Cauchy积分公式**：设区域$D$是以有限条简单闭曲线$C$为边界的有界区域。$f(z)$在$D$及$C$组成的闭区域$\bar{D}$上解析，那么在$D$内任一点$z$，
 $$f(z)=\frac{1}{2\pi i}\int_{C}\frac{f(\zeta)}{\zeta-z}\mathrm{d}z,$$
 上式称为Cauchy积分公式。
- **高阶导数公式**：设区域$D$是以有限条简单闭曲线$C$为边界的有界区域。$f(z)$在$D$及$C$组成的闭区域$\bar{D}$上解析，$f(z)$在$D$内有任意阶导数，则
 $$f^{(n)}(z)=\frac{n!}{2\pi i}\int_{C}\frac{f(\zeta)}{(\zeta-z)^{n+1}}\mathrm{d}\zeta,\ (n=1,2,\cdots).$$   
 **引理**：设$\gamma$是一曲线，并且设$\phi(\zeta)$是定义在$\zeta$的连续函数，那么
  $$ F_{n}(z)=\int_{C}\frac{\phi(\zeta)}{(\zeta-z)^{n}}\mathrm{d}\zeta\ (n=1,2,\cdots),$$
  在$\mathbb{C}-\gamma$上解析，并且$F'_ {n}(z)=nF_{n+1}(z).$
- **解析函数的无穷可微性**：设$f(z)$在$D$内解析，那么$f(z)$在$D$内有任意阶导数($0<\rho \le \rho_0$)。
- **Cauchy不等式**：设$f(z)$在以$C:\vert z-z_0\vert =\rho_0(0<\rho<+\infty)$为边界的闭圆盘上解析，那么
 $$\frac{\vert f^{(n)}(z_0)\vert}{n!}\le \frac{M(\rho)}{\rho^n}(n=0,1,2,\cdots),$$
 其中，$M(\rho)=\max\limits_{\vert z-z_0\vert=\rho}\vert f(z)\vert$和$(0<\rho \le \rho_0$)。   
 **证明**：利用高阶导数公式表示$f^{(n)}$，利用基本计算可得结论。$\blacksquare$
- **整函数**：如果函数$f(z)$在$\mathbb{C}$上解析，那么称它是一个整函数。

- **Liouville定理**：有界整函数一定恒等于常数。   
 **证明**：由Cauchy不等式，在任意的一个圆$C$内$\vert f'(z_0)\vert \le \max\limits_{\vert z-z_0\vert=\rho}\vert f(z)\vert /\rho$，而$f(z)$有界，记$\vert f(z)\vert\le M$，则$\vert f'(z_0)\vert \le m/\rho$，由于$\rho$的任意性，取$\rho\to \infty$有$\vert f'(z_0)=0$，故$f(z)$为常数。证明完毕。$\blacksquare$
- **摩勒拉定理**：如果函数$f(z)$在单连通区域$D$内连续，并且对于$D$内的任一简单曲线$C$有
 $$\int_{C}f(z)\mathrm{d}z=0,$$
 则$f(z)$在$D$内解析。

## 第四章 级数 

*目标：*
级数是研究解析函数的一个重要工具。本章主要介绍复级数和序列的基本性质、解析函数的泰勒展式、解西函数的唯一性定理、解析函数的洛朗展式以及解析函数的孤立奇点等内容。了解复级数的基本概念、收敛和发散性质，掌握复变函数项级数的收敛、一致收敛、内闭一致收敛的定义及判别方法；理解解析函数项级数的和函数的性质。理解幂级数的收敛圆、收敛半径的概念；了解幂级数和函数的解析性；理解并掌握把解析函数表示为泰勒级数的方法；熟练掌握一些初等函数的泰勒展式。理解解析函数的零点孤立性、唯一性定理。理解洛朗定理，熟练掌握将解析函数分别在指定圆环或孤立奇点的去心邻域内展成洛朗级数的方法；了解洛朗级数与泰勒级数的关系。理解孤立奇点的概念，掌握判断孤立奇点类型的方法；了解解析函数在孤立奇点去心邻域内的性质；掌握解析函数在无穷远点的性质。了解整函数与亚纯函数的概念。

*内容：*
- **定理**：设幂级数有收敛圆盘$\vert z-z_0\vert <R$，那么在$\vert z-z_0\vert <R$内，和函数
 $$f(z)=\alpha_0+\alpha_1 (z-z_0)+\alpha_2(z-z_0)^2+\cdots+\alpha_n(z-z_0)^n+\cdots$$
 解析，并且
 $$f^{(n)}(z)=n!\alpha_n+\frac{(n+1)!}{1!}\alpha_{n+1}(z-z_0)+\cdots\ \ (n=1,2,3,\cdots)$$
- **定理**：设函数$f(z)$在圆盘$U:\vert z-z_0\vert R$内解析，那么在$U$内可展成Taylor展式如下，
 $$f(z)=f(z_0)+\frac{f'(z_0)}{1!}(z-z_0)+\frac{f^{(2)}(z_0)}{2!}(z-z_0)^2+\cdots+\frac{f^{(n)}(z_0)}{n!}(z-z_0)^n+\cdots.$$
- **定理**：函数$f(z)$在点$z_0$解析的充分必要条件是它在$z_0$的某一个邻域内有幂级数展式，
 $$f(z)=\alpha_0+\alpha_1 (z-z_0)+\alpha_2(z-z_0)^2+\cdots+\alpha_n(z-z_0)^n+\cdots.$$
- **常用函数Taylor展开**：  
 1. $\mathrm{e}^{z}=1+z+\frac{z^2}{2!}+\cdots+\frac{z^n}{n!}+\cdots.$
 2. $\cos{z}=1-\frac{z^2}{2!}+\frac{z^4}{4!}-\cdots+(-1)^{k}\frac{z^{2k}}{(2k)!}+\cdots.$
 3. $\sin{z}=\frac{z}{1!}-\frac{z^3}{3!}+\frac{z^5}{5!}-\cdots+(-1)^{k-1}\frac{z^{2k-1}}{(2k-1)!}+\cdots.$
 4. $\ln{1+z}=z-\frac{z^2}{2}+\frac{z^3}{3}-\frac{z^4}{4}+\cdots+(-1)^{n-1}\frac{z^n}{n}+\cdots.$
- **零点**：设函数$f(z)$在$z_0$邻域$U$内解析，并且$f(z_0)=0$，那么$z_0$称为$f(z)$的零点。设$f(z)$在$U$内的Taylor展开是
 $$f(z)=\alpha_1(z-z_0)+\alpha_2(z-z_0)^2+\cdots+\alpha_n(z-z_0)^n+\cdots.$$
 零点可分为如下两种情况：
 1. 对于$n=1,2,\cdots$，都满足$\alpha_n=0$，那么在$U$内$f(z)$恒等于$0$.
 2. 如果$\alpha_1,\alpha_2,\cdots$不全为$0$，并且对于$m\in \mathbb{Z}^{+}$满足$\alpha_{m}\neq 0$，而$\alpha_n=0(n< m)$，则称$z_0$是$f(z)$的$m$阶零点。显然在$z_0$的邻域内$f(z)=(z-z_0)^{n}\phi (z)$，其中$\phi(z_0)\neq 0$且$\phi(z)$在$U$内解析。
 **定理**：设函数$f(z)$在$z_0$解析，并且是它的一个零点，则要么$f(z)$在$z_0$的一个邻域恒等于$0$，要么存在一个邻域内只有$z_0$一个零点。
- **引理1**：设函数$f(z)$是区域$D$内的解析函数，如果$f(z)$在$D$内的一个圆盘内恒等于$0$，则$f(z)$在$D$内恒等于$0$。
- **定理**：如果$f(z)$在区域$D$内解析，并且不恒等于$0$，则$f(z)$的每一个零点$z_0$存在一个邻域$U$满足$z_0$是$U$的唯一零点。
- **定理**：设函数$f(z)$和$g(z)$在区域$D$内解析，设$z_k(k=1,2,3,\cdots)$是$D$内互不同的点，并且点列$\{z_k\}$在$D$内有极限点，如果$f(z_k)=g(z_k)(k=1,2,\cdots)$，则在$D$内$f(z)=g(z)$。
- **Laurent级数**：函数$f(z)$的Laurent展开是
 $$f(z)=\sum\limits_{n=-\infty}^{+\infty}\beta_n(z-z_0)^n.$$
- **定理**：设函数$f(z)$在圆环$D:R_1<\vert z-z_0\vert<R_2(0\le R_1<R_2\le +\infty)$内解析，那么在$D$内
 $$f(z)=\sum\limits_{n=-\infty}^{+\infty}\alpha_{n}(z-z_0)^n,$$
 其中，$\alpha_n=\frac{1}{2\pi i}\int_{\gamma}\frac{f(z)}{(z-z_0)^{n+1}}\mathrm{d}z(n=0,\pm 1,\pm 2,\cdots)$，$\gamma$是圆$\vert z-z_0\vert=\rho$，$\rho$是满足$R_1<\rho <R_2$的任何数。
 **注1**：在上面的Laurent展开中，$\sum\limits_{n=0}^{+\infty}\beta_n(z-z_0)^n$被称为级数的解析部分，$\sum\limits_{n=-1}^{-\infty}\beta_n(z-z_0)^n$被称为级数的主要部分。
 **定理**:设级数$\sum\limits_{n=-\infty}^{+\infty}\beta_n(z-z_0)^n$在圆环$D:R_1<\vert z-z_0\vert<R_2(0\le R_1<R_2\le +\infty)$内闭一致收敛于和函数$g(z)$，则$g(z)$的Laurent展式是：
 $$g(z)=\sum\limits_{n=-\infty}^{+\infty}\beta_n(z-z_0)^n.$$
 **注2**：定理的假设下，$f(z)$的Laurent展式是唯一的。
- **孤立奇点**：设函数$f(z)$在去掉圆心的圆盘$D:0<\vert z-z_0\vert<R(0< R\le +\infty)$内解析，那么称$z_0$是$f(z)$的孤立奇点。
- **孤立奇点分类**：在孤立奇点定义的假设下，在$D$内，$f(z)$有Laurent展式
 $$f(z)=\sum\limits_{n=-\infty}^{+\infty}\alpha_n(z-z_0)^n,$$
 其中，$\alpha_n=\frac{1}{2\pi i}\int_{C_{\rho}}\frac{f(z)}{(z-z_0)^{n+1}}\mathrm{d}z(n=0,\pm 1,\pm 2,\cdots)$，$C_{\rho}$是圆$\vert z-z_0\vert =\rho(0<\rho <R)$。根据级数包含负数幂的情况可以分类：  
 1. **可去奇点**：如果$\alpha_n=0(n=0,\pm 1,\pm 2,\cdots)$，称为可去奇点。令$f(z_0)=\alpha_0$，则$f(z)$在圆盘内解析。  
 2. **$m$阶极点**：如果仅仅有限个$n<0$使得$\alpha_n=0$，那么说$z_0$是$f(z)$的极点。设$\alpha_{-m}\neq 0(m\in \mathbb{Z}^{+})$，而$\alpha_{n}=0(n<-m)$，则称$z_0$是$f(z)$的$m$阶极点。  
 3. **本性奇点**：如果有无限个$n<0$使得$\alpha_{n}\neq 0$，则称$z_0$是$f(z)$的本性奇点。
- **可去奇点等价命题**：设函数$f(z)$在$0<\vert z-z_0\vert<R(0<R\le +\infty)$内解析，那么$z_0$是$f(z)$的可去奇点的等价条件是存在极限$\lim\limits_{z\to z_0}f(z)=\alpha_0$，$\alpha_0$是一个复数。
 **注**：上面的等价条件可写成存在$0<\rho_0 \le R$，使得$f(z)$在$0<\vert z-z_0\vert \rho_0$内有界。

- **极点等价命题**：设函数$f(z)$在$0<\vert z-z_0\vert<R(0<R\le +\infty)$内解析，那么$z_0$是$f(z)$的极点的等价条件是$\lim\limits_{z\to z_0}f(z)=+\infty$。
 - **$m$阶极点等价命题**：在极点等价命题的假设下，$z_0$是$f(z)$的$m$阶极点的等价条件是$\lim\limits_{z\to z_0}(z-z_0)^{m}f(z)=\alpha_{-m}$，$\alpha_{-m}$是不等于$0$的复数，$m$是正整数。
- **本性奇点等价命题1**：设函数$f(z)$在$0<\vert z-z_0\vert<R(0<R\le +\infty)$内解析，那么$z_0$是$f(z)$的本性奇点的等价条件是$\lim\limits_{z\to z_0}f(z)$不存在(有限或者去穷)极限。
- **本性奇点等价命题2**：设函数$f(z)$在$0<\vert z-z_0\vert<R(0<R\le +\infty)$内解析，那么$z_0$是$f(z)$的本性奇点的等价条件对于任意的复数$\gamma$(有限或者无穷)，在$0<\vert z-z_0\vert<R$内存在收敛于$z_0$的点列$\{z_n\}$满足$\lim\limits_{n\to +\infty}f(z_n)=\gamma$。
- **本性奇点等价命题3**：设函数$f(z)$在$0<\vert z-z_0\vert<R(0<R\le +\infty)$内解析，那么$z_0$是$f(z)$的本性奇点的等价条件对于任意的复数$\gamma\neq \infty$，至多可能有一个反例，在$0<\vert z-z_0\vert<R$内存在收敛于$z_0$的点列$\{z_n\}$满足$f(z_n)=\gamma(n=1,2,\cdots)$。
- **无穷远点孤立奇点**：设函数$f(z)$在区域$D:R<\vert z\vert<+\infty(R\ge 0)$内解析，那么称无穷远点是$f(z)$的孤立奇点。
- **无穷远点孤立奇点分类**：在无穷远点孤立奇点定义的假设下，在区域内，$f(z)$有Laurent展式
 $$f(z)=\sum\limits_{n=-\infty}^{+\infty}\alpha_n(z)^n,$$
 其中，$\alpha_n=\frac{1}{2\pi i}\int_{C_{\rho}}\frac{f(z)}{(z)^{n+1}}\mathrm{d}z(n=0,\pm 1,\pm 2,\cdots)$，$C_{\rho}$是圆$\vert z\vert =\rho(0<\rho <R)$。根据级数包含正数幂的情况可以分类：  
  1. 如果$\alpha_n=0(n=1,2,3,\cdots)$，则$\infty$是$f(z)$的可去奇点。  
  2. 如果只有有限个$n>0$使得$\alpha_n=0$，则$\infty$是$f(z)$的极点。设$\alpha_{m}\neq 0(m\in \mathbb{Z}^{+})$，而$\alpha_{n}=0(n> m)$，则称$\infty$是$f(z)$的$m$阶极点。  
  3. 如果有无限个$n>0$使得$\alpha_{n}\neq 0$，则称$\infty$是$f(z)$的本性奇点。
- **奇点类型判定命题**：设函数$f(z)$在$R<\vert z\vert<+\infty(R\ge 0)$内解析，那么$\infty$是$f(z)$的可去奇点、极点或者本性奇点的等价条件是$\lim\limits_{z\to \infty}f(z)$存在有限、去穷或者不存在极限。
- **奇点类型判定命题**：设函数$f(z)$在$R<\vert z\vert<+\infty(R\ge 0)$内解析，那么$\infty$是$f(z)$的可去奇点的等价条件是存在$rho_0\ge R$，使得$f(z)$在$\rho_0<\vert z\vert <+\infty$内有界。

- **代数基本定理**：任何$n$次代数方程至少有一个根。
- **定理**：设$f(z)$是整函数，按照$\infty$是可去奇点、极点或本性奇点，$f(z)$恒等于一个常数，多项式或超越整函数。

- **亚纯函数**：如果函数$f(z)$在有限复平面内除去有极点外到处解析，那么它就是亚纯函数。
- **定理**：如果无穷远点$\infty$是亚纯函数$f(z)$的可去奇点或极点，那么$f(z)$是一个有理函数，即
 $$f(z)=\frac{\alpha_0+\alpha_1 z+\alpha_2 z^2+\cdots+\alpha_n z^n}{\beta_0+\beta_1 z+\beta_2 z^2+\cdots+\beta_m z^m},\ (\alpha_n,\beta_m\neq 0).$$


## 第五章 留数 

*目标：*
本章内容是对复变函数积分理论的进一步完善。主要介绍留数的概念、留数基本定理与留数的计算、应用留数计算实积分、辐角原理、儒歇定理等内容。理解留数的定义和留数基本定理，熟练掌握留数的计算方法；掌握利用留数定理计算函数沿闭曲线的积分；熟练掌握用留数定理计算三类实积分，了解应用多值函数的留数计算实积分；了解对数留数的概念，理解辐角原理、儒歇定理，熟练掌握求解析函数在指定区域内的零点个数的方法。

*内容：*
- **留数**：设函数$f(z)$在区域$0<\vert z-z_0\vert <R$解析，选取$0< r <R$作圆$C:\vert z-z_0\vert =r$，如果$z_0$是$f(z)$的孤立奇点，则定义$f(z)$在孤立奇点$z_0$的留数是
 $$\frac{1}{2\pi i}\int_{C}f(z)\mathrm{d}z.$$
 记作$\mathrm{Res }{(f,z_0)}$，其中$C$是沿逆时针方向。
 **注**：如果奇点是可去奇点，则留数的值是$0$.
- **定理**：设$D$是复平面的有界区域，其边界$C$由有限条简单闭曲线组成。如果$f(z)$在$D$内除去孤立奇点$z_1,z_2,\cdots z_n$外每一点都解析，并且在$C$上每一点也解析，那么有
 $$\int_{C}f(z)\mathrm{d}z=2\pi i\sum\limits_{k=1}^{n}\mathrm{Res}(f,z_k),$$
 其中$C$的积分沿$D$的正方向。
- **一阶极点的留数计算**：设$z_0$是$f(z)$在圆盘内的一阶极点，则留数是
 $$\mathrm{Res}(f,z_0)=\lim\limits_{z\to z_0}(z-z_0)f(z).$$
 - 如果在$z_0$的去心圆盘内$f(z)=P(z)/Q(z)$，其中$P(z),Q(z)$在圆盘内解析，并且$P(z_0)\neq 0$，$z_0$是$Q(z)$的一阶零点，$Q(z)$在圆盘内没有其他零点，则有
 $$\mathrm{Res}(f,z_0)=\lim\limits_{z\to z_0}(z-z_0)f(z)=\lim\limits_{z\to z_0}(z-z_0)\frac{P(z)}{Q(z)-Q(z_0)}=\frac{P(z_0)}{Q'(z_0)}.$$
- **高阶极点的留数计算**：设$z_0$是$f(z)$在圆盘内的$k$阶极点，则留数是
 $$\mathrm{Res}(f,z_0)=\frac{1}{(k-1)!}\lim\limits_{z\to z_0}\frac{\mathrm{d}^{k-1}}{\mathrm{d}z^{k-1}}\big{(}(z-z_0)^{k}f(z)\big{)}.$$

- **留数应用 1**：计算$I=\int_{0}^{2\pi}R(\sin{t},\cos{t})\mathrm{d}t$，其中$R(x,y)$是有理分式，并且在单位圆上分母不为$0$。方法是做$z=\mathrm{e}^{it}$带入方程，然后用留数定理求对应的积分。
- **留数应用 2**：计算$I=\int_{-\infty}^{+\infty}R(x)\mathrm{d}x$，其中$R(x)$是有理分式，并且分母在实轴上不为$0$，分母的次数比分子的次数至少高$2$次。方法是。
- **引理**：设$f(z)$在闭区间$\theta_1\le \mathrm{Arg }z\le \theta_2$，$r_0\le \vert z\vert <+\infty$，($r_0\ge 0,0\le \theta_1< \theta_2 \le \pi$)上连续的复变函数，并且设$\Gamma_{r}$是以$O$为圆心，$r$为半径的圆弧在这个闭区间上的一段($r\ge r_0$)，如果$z$在闭区间上$\lim\limits_{x\to \infty} f(z)=0$，那么有
 $$\lim\limits_{r\to +\infty}\int_{\Gamma_{r}}f(z)\mathrm{e}^{iz}\mathrm{d}z=0$$
- **留数应用 3**：计算$I=\int_{-\infty}^{+\infty}f(x)\mathrm{e}^{ix}\mathrm{d}x$，其中$f(z)$在$\Im{z}\ge 0$上可能有有限个奇点外，在其他每一点解析，且当$z$在$\Im{z}\ge 0$上时，$\lim\limits_{z\to \infty}f(z)=0$。

- **留数应用 4**：计算积分$I=\int_{0}^{+\infty}\frac{R(x)}{x^{\alpha}}\mathrm{d}x$，其中$0<\alpha<1$，$R(x)$是有理分式，分母的次数比分子高。

- **留数应用 5**：计算积分$I=\int_{0}^{+\infty}R(x)\ln{x}\mathrm{d}x$，其中$R(x)$是有理分式，分母的次数比分子至少高$2$次。

- **留数应用 6**：有些根式$\big{(}(x-a)^k(x-b)^{n-k}\big{)}^{\frac{1}{n}}$或$\big{(}(x-a)^k(x-b)^{n-k}\big{)}^{-\frac{1}{n}}$与有理分式的乘积在某些有限区域上的积分。

- **引理**：设$f(z)$是有界区域$D$上的亚纯函数，$f(z)$在$D$的边界$C$上的每一点解析，且在$C$上没有零点，那么$f(z)$在$D$内至多有有限个零点和极点。
- **定理**：设$D$为复平面有界区域，边界$C$是有限条闭曲线组成。$f(z)$是$D$上的亚纯函数，在$C$上的每一点解析，且在$C$上没有零点，那么
 $$\frac{1}{2\pi i}\int_{C}\frac{f'(z)}{f(z)}\mathrm{d}z=N-P,$$
 其中，$N$和$P$是$f(z)$在$D$内零点和极点的总数，并且每个$k$阶零点或者极点算作$k$个零点和极点。
 **定理**：在上述定理的假设下，有
 $$N-P=\frac{1}{2\pi }\Delta_{C}\arg{f(z)}=\frac{1}{2\pi }\sum\limits_{j=1}^{n}\Delta_{C_j}\arg{f(z)}$$
 其中，$C_1,C_2,\cdots,C_n$表示构成$C$的所有闭曲线，方向关于$D$的正方向，$\Delta_{C}\arg{f(z)}$表示$z$沿着$C$正向绕一周时，$\arg{f(z)}$连续变动的增量。

- **Rouche定理**：设$D$是复平面的一个有界区域，边界$C$是有限条简单闭曲线，函数$f(z)$和$g(z)$在$D$和$C$组成的闭区域上解析，并且在$C$上，$\vert g(z)\vert <\vert f(z)\vert$，那么在$D$上，$f(z)$和$f(z)+g(z)$的零点个数相同。


## 第六章 保形映射 

*目标：*
本章内容涉及解析函数的几何理论。主要介绍单叶解析函数的映射性质、导数的几何意义、分式线性函数及其映射性质、黎曼定理等内容。理解单叶解析函数的性质，了解解析变换的特性（保域性、保角性、共形性）；理解分式线性变换的映射性质，掌握将区域 D 共形映射为区域 G 的分式线形变换；理解最大模原理、施瓦茨引理，了解黎曼定理及边界对应定理；理解幂函数、指数函数、根式函数、对数函数的映射性质，熟练掌握它们所构成的共形映射；会求两个指定区域之间的共形变换。

*内容：*

- **单叶解析函数**：设函数$f(z)$在区域$D$内解析，并且在$D$内不同两点的取值不同，那么函数$f(z)$称为$D$上的单叶解析函数。

