---
layout: post
title:  "概率统计"
date:   2020-01-20 02:34:20 +0800
categories: math
tags: probability
---

# 概率与统计

* any list
{:toc}

## 一. 概率论

### 1. 随机事件和样本空间
理解随机事件和样本空间的概念，掌握事件之间的关系与运算；理解并熟练掌握概率的古典定义；理解几何概率，概率的统计定义及公理化定义；熟练掌握概率的基本性质，会用于计算；理解并掌握条件概率的定义，事件独立性。熟练掌握乘法公式、全概率公式与贝叶斯公式及其应用；熟练掌握 Bernoulli 概型。

- **概率(古典定义)**：随机事件$A$发生可能性大小的度量（数值）称为$A$发生的概率，记作$P(A)$。

- **古典概型**：样本空间的元素只有有限个，设为$n$个元素并且记作$\omega_1,\omega_2,\cdots,\omega_n$。每个时间出现的概率相等，即
 \begin{equation}
 P(\omega_1)=P(\omega_2)=\cdots=P(\omega_n).
 \end{equation}
 称这种数学模型为古典概型。

- **几何概率**：在一个面积为$S_{\Omega}$的区域$\Omega$中，有任意个小区域$A$，如果它的面积是$S_{A}$，则投点落入$A$中的可能性大小与$S_{A}$成正比，而与$A$的位置和形状无关，记作这个随机事件是$A$，则
 \begin{equation}
 P(A)=\frac{S_A}{S_{\Omega}}
 \end{equation}
 称这一类概率为几何概率。

- **概率(严格定义)**：概率是定义在$\sigma$-代数$\mathcal{F}$上的一个非负的规范的可列可加的集函数。即对于概率$P$有
 1. 非负性：$P(A)\ge 0$，对于$A\in \mathcal{F}$;
 2. 规范性：$P(\Omega)=1$;
 3. 可列可加性：若$A_i\in \mathcal{F},i=1,2,\cdots$，且$A_iA_j=\varnothing$($i\neq j$)，则
 \begin{equation}
 P\big{(}\bigcup\limits_{i=1}^{+\infty}A_i\big{)}=\sum_{i=1}^{+\infty}P(A_i).
 \end{equation}

- **下连续的**：对于$\mathcal{F}$上的集合函数$P$，若对$\mathcal{F}$中的任一单调不减集合序列$\{A_{n}\}$有
 \begin{equation}
 \lim_{n\to +\infty}P(A_n)=P(\lim_{n\to +\infty}A_n),
 \end{equation}
 则称集合函数$P$在$\mathcal{F}$上是下连续的，其中$\lim\limits_{n\to +\infty}A_n=\bigcup\limits_{n=1}^{+\infty}A_n$。

- **定理**：若$P$是$\mathcal{F}$上的非负的规范的集函数，则$P$具有可列可加性的充分必要条件是
 1. $P$是有限可加的；
 2. $P$在$\mathcal{F}$上是下连续的。

- **条件概率**：若$(\Omega,\mathcal{F},P)$是一个概率空间，$B\in \mathcal{F}$，且$P(B)>0$，则对于任意$A\in \mathcal{F}$称
 \begin{equation}
 P(A\vert B)=\frac{P(AB)}{P(B)}
 \end{equation}
 为已知事件$B$发生的情况下，事件$A$发生的概率。

- **全概率公式**：设$B_1,B_2,\cdots$是一列互不相容的事件，且有
 \begin{equation}
 \bigcup_{i=1}^{+\infty}B_i=\Omega,\ \ P(B_i)>0,\ \ i=1,2,\cdots
 \end{equation}
 则对任一事件$A$有
 \begin{equation}
 P(A)=\sum_{i=1}^{+\infty}P(B_i)P(A\vert B_i).
 \end{equation}

- **Bayes公式**：设$B_1,B_2,\cdots$是一列互不相容的事件，且有
 \begin{equation}
 \bigcup_{i=1}^{+\infty}B_i=\Omega,\ \ P(B_i)>0,\ \ i=1,2,\cdots
 \end{equation}
 则对任一事件$A$有
 \begin{equation}
 P(B_i\vert A)=\frac{P(B_i)P(A\vert B_i)}{\sum\limits_{i=1}^{+\infty}P(B_i)P(A\vert B_i)}.
 \end{equation}

- **一般概率乘法公式**：
 \begin{equation}
 P(AB)=P(A)P(B\vert A).
 \end{equation}

- **独立的**：如果两个事件$A,B$满足
 \begin{equation}
 P(AB)=P(A)P(B),
 \end{equation}
 则称事件$A,B$是相互独立的。

 **$n$个事件独立**：如果$n$个事件$A_1,A_2,\cdots,A_n$，对于任意的$k\le n$，任意一组$1\le i_1\le i_2\le\cdots\le i_k$满足
 \begin{equation}
 P(A_{i_1}A_{i_2}\cdots A_{i_k})=P(A_{i_1})P(A_{i_2})\cdots P(A_{i_k}),
 \end{equation}
 则称事件$A_1,A_2,\cdots,A_n$是相互独立的。

- **Bernoulli 概型**：如果实验$E$只有两种可能结果$A$和$\bar{A}$，并且$P(A)=p$，而$P(\bar{A})=1-p=q$，把$E$独立重复$n$次的实验称为$n$重Bernoulli试验，也叫做Bernoulli实概型。记$n$次实验中$A$出现$k$次是事件$B_k$，则有概率
 \begin{equation}
 P(B_k)=
 \begin{pmatrix}
 n\newline
 k
 \end{pmatrix}
 p^{k}q^{n-k},\ \ (0\le k\le n).
 \end{equation}



### 2. 随机变量
理解随机变量的概念；理解并熟练掌握分布函数、分布律、概率密度等概念及其性质，掌握分布函数与分布律，分布函数与概率密度之间的关系；掌握二项分布、Poisson 分布、均匀分布、指数分布，熟练掌握正态分布，会查标准正态分布表；熟练掌握随机变量函数分布的求法。

- **离散型随机变量**：定义在样本空间$\Omega$上，取值于实数域$\mathbb{R}$，且只有有限个或者可数个值的变量$\xi=\xi(\omega)$，称作是一维(实值)离散型随机变量，简称离散型随机变量。

- **分布律**：把如下表格称为分布律或者分布列：

 $\xi$ | $a_1$ | $a_2$ | $\cdots$ |
 :-: | :-: | :-: | :-: |
 $p_i$ | $p_1$ | $p_2$ | $\cdots$ |

- **二项分布**：Bernoulli概型对应的分布列称为二项分布，即
 \begin{equation}
 b(k;n,p)=
 \begin{pmatrix}
 n\newline
 k
 \end{pmatrix}
 p^{k}q^{n-k}.
 \end{equation}

- **两点分布**：对于二项分布如果$n=1$，称这个分布是两点分布，也成为$0-1$分布。
- **单点分布**：随机变量$\xi$分布列为
 \begin{equation}
 P(\xi=a)=1
 \end{equation}
 的分布称为单点分布或退化分布。
- **Poisson分布**：随机变量$\xi$分布列为
 \begin{equation}
 P(\xi=k)=\frac{\lambda^k}{k!}e^{-\lambda},\ \ k=0,1,2,\cdots
 \end{equation}
 其中$\lambda>0$是一个常数，这个分布称为Poisson分布。

- **Poisson定理**：在$n$重Bernoulli试验中，事件$A$在一次试验中出现的概率是$p_n$，如果当$n\to +\infty$时，$np_n\to \lambda$($\lambda$是常数)，则有
 \begin{equation}
 \lim_{n\to +\infty}b(k;n,p_n)=\frac{\lambda^k}{k!}e^{-\lambda},\ \ k=0,1,2,\cdots.
 \end{equation}

- **$n$为随机变量**：设$\xi_1,\xi_2,\cdots,\xi_n$是样本空间$\Omega$上的$n$个离散随机变量，则称$n$维向量$(\xi_1,\xi_2,\cdots,\xi_n)$是$\Omega$上一个$n$维离散型随机变量。

- **联合分布列**：设$(\xi,\eta)$是二维离散型随机变量，一切可能取值是$(a_i,b_j)$,$i,j=1,2,\cdots$，令
 \begin{equation}
 p_{ij}=P(\xi=a_i,\eta=b_j),\ \ i,j=1,2,\cdots
 \end{equation}
 称$(p_{ij},i,j=1,2,\cdots)$是二维离散型随机变量$(\xi,\eta)$的联合分布列。

- **相互独立**：设离散型随机变量$\xi$的可能取值为$a_i(i=1,2,\cdots)$，$\eta$的可能取值是$b_j(j=1,2,\cdots)$，如果对任意的$a_i,b_j$有
 \begin{equation}
 P(\xi=a_i,\eta=b_j)=P(\xi=a_i)P(\eta=b_j)
 \end{equation}
 则称随机变量$\xi$和$\eta$相互独立。

- **Poisson分布可加性**：设$\xi,\eta$是两个独立随机变量，他们服从参数为$\lambda_1$和$\lambda_2$的Poisson分布，则$\zeta=\xi+\eta$服从参数是$\lambda_1+\lambda_2$的Poisson分布。

- **概率分布函数**：定义在样本空间$\Omega$上，取值于实数域的函数$\xi(\omega)$称为是样本空间$\Omega$上的随机变量，并称
 \begin{equation}
 F(x)=P(\xi(\omega)\le x),\ x\in (-\infty,+\infty)
 \end{equation}
 是随机变量$\xi(\omega)$的概率分布函数，简称分布函数或者分布。

- **指数分布**：随机变量$\eta$的分布函数
 \begin{equation}
 F(t)=P(\eta\le t)=
 \begin{cases}
 1-e^{-\lambda t},\ \ &t\ge 0,\newline
 0,&t<0.
 \end{cases}
 \end{equation}
 称这个分布函数是参数是$\lambda$的指数分布。

- **密度**：设随机变量$\xi(\omega)$的分布函数是$F(x)$，如果存在函数$p(x)$使得任意$x$有
 \begin{equation}
 F(x)=\int_{-\infty}^{x}p(y)dy,
 \end{equation}
 则称$\xi(\omega)$为连续性随机变量，$F(x)$是连续型分布函数，$p(x)$是$F(x)$的概率密度函数或者密度。

- **正态分布**：正态分布$N(\mu,\sigma)$的密度函数是
 \begin{equation}
 p(x)=\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x-\mu)^2}{2\sigma^2}},\ -\infty< x< +\infty,
 \end{equation}
 分布函数是
 \begin{equation}
 F(x)=\frac{1}{\sqrt{2\pi}\sigma}\int_{-\infty}^{x}e^{\frac{(y-\mu)^2}{2\sigma^2}}dy,\ \ -\infty< x< +\infty,
 \end{equation}
 其中，$\mu,\sigma$($\sigma>0$)是两个常数。  
 **注**：$\mu=0,\sigma=1$的正态分布称为标准正态分布。

- **$n$维随机变量**：设$\xi_1(\omega),\xi_2(\omega),\cdots,\xi_n(\omega)$是定义在同一个样本空间$\Omega$上的随机变量，则$n$维向量空间$(\xi_1(\omega),\xi_{2}(\omega),\cdots,\xi_{n}(\omega))$称为是样本空间$\Omega$上的$n$维随机变量。并称$n$元函数
 \begin{equation}
 F(x_1,x_2,\cdots,x_n)=P\big{(}\xi_1(\omega)\le x_1,\xi_2(\omega)\le x_2,\cdots,\xi_{n}(\omega)\le x_n\big{)}
 \end{equation}
 是$n$维随机变量$(\xi_1(\omega),\xi_2(\omega),\cdots,\xi_{n}(\omega))$的联合分布函数。

- **二维随机变量密度**：设$F(x,y)$是一个联合分布函数，若存在函数$p(x,y)$，使得任意的$(x,y)$有
 \begin{equation}
 F(x,y)=\int_{-\infty}^{x}\int_{-\infty}^{y}p(u,v)dudv,
 \end{equation}
 则称$p(x,y)$是$F(x,y)$的联合概率密度函数或者简称密度。

- **定理**：设$\xi$是一个连续型随机变量，密度函数是$p(x)$，又函数$y=f(x)$严格单调，其反函数$h(y)$有连续导数，则$\eta=f(\xi)$也是连续型随机变量，且其密度是
 \begin{equation}
 \varphi(y)=
 \begin{cases}
 p[h(y)]\cdot \vert h'(y)\vert,\ \ &\alpha< y< \beta\newline
 0,&\text{其他}
 \end{cases}
 \end{equation}
 其中
 \begin{equation}
 \alpha =\min\{f(-\infty),f(+\infty)\},\ \ \beta =\max\{f(-\infty),f(+\infty)\}.
 \end{equation}



### 3. 数学期望和方差
熟练掌握随机变量的数学期望、方差及其求法。掌握特征函数的定义及性质，特征函数与期望和方差之间的关系，理解反演公式和唯一性定理。

- **离散数学期望**：如果离散型随机变量$\xi$可能取值为$a_i$$(i=1,2,\cdots)$，其分布列为$p_i(i=1,2,\cdots)$，则当
 \begin{equation}
 \sum_{i=1}^{+\infty}\vert a_i\vert p_i<+\infty,
 \end{equation}
 则称$\xi$存在数学期望，并且数学期望是
 \begin{equation}
 E{\xi}=\sum_{i=1}^{+\infty} a_i p_i.
 \end{equation}
 如果
 \begin{equation}
 \sum_{i=1}^{+\infty}\vert a_i\vert p_i = +\infty,
 \end{equation}
 则称$\xi$的数学期望不存在。

- **定理**：如果$\xi$是离散型随机变量，分布列是$P(\xi=a_i)=p_i$，又$g(x)$是实变量$x$的单值函数，如果$\sum_\limits{i=1}^{+\infty}\vert g(a_i)\vert p_i< +\infty$，则有
 \begin{equation}
 Eg(\xi)=\sum_{i=1}^{+\infty}g(a_i)p_i.
 \end{equation}

- **定理**：如果$(\xi,\eta)$是二维离散型随机变量，联合分布列是
 \begin{equation}
 P(\xi=a_i,\eta=b_j)=p_{ij},\ \ i,j=1,2,\cdots
 \end{equation}
 又$g(x,y)$是实变量$x,y$的单值函数，如果
 \begin{equation}
 \sum_{i=1}^{+\infty}\sum_{j=1}^{+\infty}\vert g(a_i,b_j)\vert p_{ij}< +\infty
 \end{equation}
 则有
 \begin{equation}
 Eg(\xi,\eta)=\sum_{i=1}^{+\infty}\sum_{j=1}^{+\infty} g(a_i,b_j)p_{ij}.
 \end{equation}

- **离散方差**：设$\xi$是一个离散型随机变量，数学期望$E\xi$存在，如果$E(\xi-E\xi)^2$存在，则称$E(\xi-E\xi)^2$为随机变量$\xi$的方差，并且记作$D\xi$或者$\mathrm{Var}\xi$。方程的平方根$\sqrt{D\xi}$称为标准差，记作$\sigma$。  
 **方差与期望的关系**：设离散随机变量$\xi$的期望是$E\xi$方差是$D\xi$，则有
 \begin{equation}
 D\xi=E(\xi-E\xi)^2=E\big{(}\xi^2+(E\xi)^2-2\xi E\xi\big{)}=E\xi^2-(E\xi)^2.
 \end{equation}
 **方差的性质**：设$\xi$是离散型随机变量，则有
 1. $D(C\xi)=C^2D\xi$.
 2. $\xi,\eta$是两个相互独立的随机变量，且$D\xi,D\eta$存在，则
 \begin{equation}
 D(\xi+\eta)=D\xi +D\eta.
 \end{equation}

- **条件期望**：如果随机变量$\xi$在"$\eta=b_j$"条件下的条件分布列为$P_{i\vert j}$，又
 \begin{equation}
 \sum_{i=1}^{+\infty}\vert a_i\vert p_{i\vert j}< +\infty,
 \end{equation}
 则称$\sum\limits_{i=1}^{+\infty}a_ip_{i\vert j}$为$\eta$在"$\eta=b_j$"条件下的条件数学期望，简称条件期望，记作$E\{\xi\vert \eta=b_j\}$.





- **连续随机变量期望**：设$\xi$是一个连续型随机变量，密度函数是$p(x)$，当
 \begin{equation}
 \int_{-\infty}^{+\infty}\vert x\vert p(x)dx< +\infty,
 \end{equation}
 称$\xi$的数学期望存在，且
 \begin{equation}
 E\xi=\int_{-\infty}^{+\infty}xp(x)dx.
 \end{equation}

- **Cauchy分布**：Cauchy分布的密度函数是
 \begin{equation}
 p(x)=\frac{1}{\pi}\frac{1}{1+x^2}.
 \end{equation}  
 **注**：期望不存在。

- **定理**：设$\xi$是连续型随机变量，密度函数是$p(x)$，如果$f(x)$是实变量$x$的函数，并且
 \begin{equation}
 \int_{-\infty}^{+\infty}=\vert f(x)\vert p(x)dx< +\infty
 \end{equation}
 则有
 \begin{equation}
 Ef(\xi)=\int_{-\infty}^{+\infty}f(x)p(x)dx.
 \end{equation}

- **定理**：设$(\xi,\eta)$是二维连续型随机变量，密度函数是$p(x,y)$，又$f(x,y)$是二元函数，则随机变量$\zeta=f(\xi,\eta)$的数学期望是
 \begin{equation}
 E\zeta=Ef(\xi,\eta)=\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty}f(x,y)p(x,y)dxdy.
 \end{equation}
 当然这里也要求上面的积分绝对收敛。

- **方差**：对于随机变量$\xi$，如果$E(\xi-E\xi)^2$存在，则称$E(\xi-E\xi)^2$是随机变量$\xi$的方差，记作$D\xi$或者$Var\xi$，并称$\sqrt{D\xi}$是$\xi$的标准差。

- **Chebyshev(Чебышев)不等式**：任意的随机变量$\xi$，若$E\xi=a$，且$D\xi$存在，则对于任意的常数$\varepsilon>0$，有
 \begin{equation}
 P(\vert \xi-a\vert \ge \varepsilon)\le \frac{D\xi}{\varepsilon^2}.
 \end{equation}



### 4. 二维随机变量
理解二维随机变量及其分布的定义，会求边缘分布，掌握随机变量的独立性；掌握二维随机变量期望、方差、协方差、相关系数及其性质；理解条件分布和条件数学期望；会求二维随机变量函数的分布；理解二维随机变量特征函数及其性质；了解三维及三维以上随机变量的定义和分布； 掌握$n$维正态分布定义及性质，$ \chi^2 $-分布、$t$-分布和$F$-分布。

- **$\chi^2$分布**：自由度为$n$的$\chi^2$分布的密度函数是
 \begin{equation}
 p(x)=
 \begin{cases}
 \frac{1}{2^{n/2}\Gamma(n/2)}x^{\frac{n}{2}-1}e^{-\frac{x}{2}},\ \ & x\ge 0 \newline
 0, & x<0.
 \end{cases}
 \end{equation}

- **$\Gamma$分布**：如果随机变量$\xi$具有密度函数
 \begin{equation}
 p(x)=
 \begin{cases}
 \frac{\lambda^{\alpha}}{\Gamma(\alpha)}x^{\alpha -1}e^{-\lambda x},\ \ & x\ge 0\newline
 0, &x<0
 \end{cases}
 \end{equation}
 则称$\xi$是参数为$(\alpha,\lambda)$的$\Gamma$分布的随机变量，相应分布称作参数是$(\alpha,\lambda)$的$\Gamma$分布，记作$Ga(\alpha,\lambda)$。

- **$F$分布**：参数为$n,m$的$F$分布$F(n,m)$的密度函数是
 \begin{equation}
 p(x)=\frac{\Gamma(\frac{m+n}{2})}{\Gamma(\frac{n}{2})\Gamma(\frac{m}{2})}n^{\frac{n}{2}}m^{\frac{m}{2}}\frac{y^{\frac{n}{2}-1}}{(ny+m)^{\frac{m+n}{2}}}.
 \end{equation}

- **$\beta$分布**：如果随机变量$\xi$的密度函数是
 \begin{equation}
 p(x)=
 \begin{cases}
 \frac{\Gamma(a+b)}{\Gamma(a)\Gamma(b)}x^{a-1}(1-x)^{b-1},\ \ &0< x< 1\newline
 0,& \text{其他}
 \end{cases}
 \end{equation}
 则称$\xi$服从$\beta$分布，记作$\xi \sim Be(a,b)$，其中$a>0,b>0$。

- **变量变换原理**：设$(\xi,\eta)$的联合密度函数是$p(x,y)$，如果函数
 \begin{equation}
 \begin{cases}
 \mu =g_1(x,y)\newline
 \nu =g_2(x,y)
 \end{cases}
 \end{equation}
 有连续偏导数，且存在唯一的反函数
 \begin{equation}
 \begin{cases}
 x=x(\mu,\nu)\newline
 y=y(\mu,\nu)
 \end{cases},
 \end{equation}
 其变换的Jacobi行列式
 \begin{equation}
 J=\frac{\partial(x,y)}{\partial (\mu,\nu)}=
 \begin{vmatrix}
 \frac{\partial x}{\partial \mu} & \frac{\partial x}{\partial \nu}\newline
 \frac{\partial y}{\partial \mu} & \frac{\partial y}{\partial \nu}
 \end{vmatrix}
 \neq 0
 \end{equation}
 若
 \begin{equation}
 \begin{cases}
 U=g_1(\xi,\eta)\newline
 V=g_2(\xi,\eta)
 \end{cases}
 \end{equation}
 则$(U,V)$的联合密度函数是
 \begin{equation}
 p(\mu,\nu)=p(x(\mu,\nu),y(\mu,\nu))\vert J\vert.
 \end{equation}

- **$t$分布**：自由度是$n$的$t$分布的密度函数是
 \begin{equation}
 p(x)=\frac{\Gamma(\frac{n+1}{2})}{\sqrt{n\pi}\Gamma(\frac{n}{2})}(1+\frac{y^2}{n})^{-\frac{n+1}{2}}.
 \end{equation}

- **协方差**：设$(\xi,\eta)$是二维随机变量，且
 \begin{equation}
 E\vert (\xi-E\xi)(\eta-E\eta)\vert < +\infty
 \end{equation}
 则称$E(\xi-E\xi)(\eta-E\eta)$为$\xi$和$\eta$的协方差，记作$Cov{(\xi,\eta)}$，即
 \begin{equation}
 Cov(\xi,\eta)=E(\xi-E\xi)(\eta-E\eta).
 \end{equation}  
 **注**：协方差$Cov(\xi,\eta)$关于$\xi,\eta$是双线性函数。

- **相关系数**：设$(\xi,\eta)$是二维随机变量，且
 \begin{equation}
 E\Big{\vert} \frac{(\xi-E\xi)}{\sqrt{D\xi}}\cdot\frac{(\eta-E\eta)}{\sqrt{D\eta}}\Big{\vert} < +\infty,
 \end{equation}
 则称
 \begin{equation}
 Cov(\xi^{ * },\eta^{ * })=E(\xi^{ * }-E\xi^{ * })(\eta^{ * }-E\eta^{ * })=E\Big{(}\frac{\xi-E\xi}{\sqrt{D\xi}}\cdot \frac{\eta-E\eta}{\sqrt{D\eta}}\Big{)}=\frac{Cov(\xi,\eta)}{\sqrt{D\xi\cdot D\eta}}.
 \end{equation}
 其中，$\xi^{ * }$和$\eta^{* }$定义为
 \begin{equation}
 \xi^{ * }=\frac{\xi -E\xi}{\sqrt{D\xi}},\ \ \eta^{ * }=\frac{\eta -E\eta}{\sqrt{D\eta}}.
 \end{equation}

- **引理**：设$(\xi,\eta)$是一个二维随机变量，且$E\xi^2< +\infty$,$E\eta^2< +\infty$，则有
 \begin{equation}
 \vert E(\xi\eta)\vert ^2\le E\xi^2\cdot E\eta^2.
 \end{equation}

- **定理**：设二维随机变量$(\xi,\eta)$的两个分量$\xi$和$\eta$的相关系数是$\rho$，则有
 1. $\vert \rho\vert \le 1$；
 2. $\vert \rho \vert =1$的充分必要条件是以概率$1$线性相关，即存在常数$a,b$有
 \begin{equation}
 P(\eta=a\xi+b)=1.
 \end{equation}

- **矩**：随机变量$\xi$的$k$阶矩是$E\xi^k$，$k$阶中心距是$E(\xi-E\xi)^k$，关于$a$点的$p$阶矩是$E(\xi-a)^p$。对于二维随机变量$(\xi_1,\xi_2)$，它的$k+l$阶混合矩是$E(\xi_1^k\cdot\xi_2^l)$，$k+l$阶中心混合矩是$E(\xi_1-E\xi_1)^k(\xi_2-E\xi_2)^l$.

- **协方差矩阵**：矩阵$B=(b_{ij}) _ {i,j=1,2}$，且$b_{ij}=Cov{\xi_1,\xi_j}$，则称$B$是$\xi$的协方差矩阵。

- **条件期望**：设随机变量$\xi$在$(\eta=y)$发生的条件下的条件密度是$p_{\xi\vert \eta}(x\vert y)$，且
 \begin{equation}
 \int_{-\infty}^{+\infty}\vert x\vert p_{\xi\vert \eta}(x\vert y)dx< +\infty,
 \end{equation}
 则称
 \begin{equation}
 E(\xi\vert \eta=y)=\int_{-\infty}^{+\infty}xp_{\xi\vert \eta}(x\vert y)dx
 \end{equation}
 是$\xi$在$(\eta=y)$发生的条件下的条件数学期望，简称条件期望。


### 5. 大数定律和中心极限定律
理解大数定律和中心极限定理的统计背景，意义及其应用，了解依概率$1$ 收敛，依概率收敛及依分布收敛的意义和相互关系。

- **Bernoulli定理**：设$\mu_{n}$是$n$重Bernoulli试验中事件$A$出现的次数，又$A$在每次试验中出现的概率是$p(0< p <1)$，则对任意的$\varepsilon>0$，有
 \begin{equation}
 \lim_{n\to +\infty}P\Big{(}\Big{\vert} \frac{\mu_n}{n}-p\Big{\vert} < \varepsilon\Big{)}=1.
 \end{equation}

- **服从大数定理**：若$\xi_1,\xi_2,\cdots,\xi_n,\cdots$是随机变量序列，如果存在常数列$a_1,a_2,\cdots$，使得任意的$\varepsilon>0$有
 \begin{equation}
 \lim_{n\to +\infty}P\Big{(}\Big{\vert}\frac{\sum_{i=1}^{n}\xi_i}{n}-a_n\Big{\vert}< \varepsilon\Big{)}=1,
 \end{equation}
 则称随机变量序列$\{\xi_n\}$服从大数定律。

- **Chebyshev大数定律**：设$\xi_1,\xi_2,\cdots$是一列两两不相关的随机变量，又设他们的方差有界，即存在常数$M>0$使得
 \begin{equation}
 D\xi_i\le M,\ \ i=1,2,\cdots
 \end{equation}
 则对于任意的$\varepsilon>0$，有
 \begin{equation}
 \lim_{n\to +\infty}P\Big{(}\Big{\vert}\frac{1}{n}\sum_{i=1}^{n}\xi_i-\frac{1}{n}\sum_{i=1}^{n}E\xi_i\Big{\vert}<\varepsilon\Big{)}=1.
 \end{equation}

- **Markov大数定律**：对随机变量$\xi_n$，如果有
 \begin{equation}
 \frac{1}{n^2}D(\sum_{i=1}^{n}\xi_i^2)\to 0
 \end{equation}
 则$\xi_n$服从大数定律，即对任意的$\varepsilon >0$，有
 \begin{equation}
 \lim_{n\to +\infty}P\Big{(}\Big{\vert} \frac{1}{n}\sum_{i=1}^{n}\xi_i-\frac{1}{n}\sum_{i=1}^{n}E\xi_i\Big{\vert} < \varepsilon\Big{)} = 1.
 \end{equation}

- **Khinchin(辛钦)大数定律**：设$\xi_1,\xi_2,\cdots$是一个独立同分布的随机变量，且数学期望存在是：
 \begin{equation}
 E\xi_1=a,\ \ i=1,2,\cdots
 \end{equation}
 则对于任意$\varepsilon >0$，有
 \begin{equation}
 \lim_{n\to+\infty}P\Big{(}\Big{\vert}\frac{1}{n}\sum_{i=1}^{n}\xi_i-a\Big{\vert}<\varepsilon \Big{)}=1.
 \end{equation}

- **依概率收敛**：设有一列随机变量$\eta,\eta_1,\eta_2,\cdots$,如果对于任意$\varepsilon >0$，有
 \begin{equation}
 \lim_{n\to +\infty}P(\vert \eta_n-\eta\vert <\varepsilon)=1
 \end{equation}
 则称随机变量序列$\eta_n$以概率收敛于$\eta$，记作
 \begin{equation}
 \lim_{n\to +\infty}\eta_n\overset{P}{=}\eta,
 \end{equation}
 或者
 \begin{equation}
 \eta_{n}\stackrel{P}{\longrightarrow}\eta,\ \ (n\to +\infty).
 \end{equation}


- **弱收敛**：设$F(x),F_1(x),F_2(x),\cdots$是一列分布函数，如果对于$F(x)$的每一个连续点$x$都有
 \begin{equation}
 \lim_{n\to +\infty}F_{n}(x)=F(x),
 \end{equation}
 则称分布函数列$F_n(x)$弱收敛于分布函数$F(x)$，并且记作
 \begin{equation}
 F_n(x)\overset{W}{\longrightarrow}F(x).
 \end{equation}

- **定理**：若随机变量序列$\eta_1,\eta_2,\cdots$依概率收敛于随机变量$\eta$，即
 \begin{equation}
 \eta_{n}\overset{P}{\longrightarrow}\eta,\ \ (n\to +\infty)
 \end{equation}
 则相应的分布函数列$F_1(x),F_2(x),\cdots$弱收敛于分布函数$F(x)$，即
 \begin{equation}
 F_n(x)\overset{W}{\longrightarrow}F(x),\ \ (n\to +\infty).
 \end{equation}

- **定理**：分布函数列$F_n(x)$弱收敛于分布函数$F(x)$的充分必要条件是相应的特征函数列$\varphi_n(t)$收敛于$F(x)$的特征函数$\varphi(t)$。

- **定理**：设$\xi_{1n},\xi_{2n},\cdots,\xi_{kn}$是$k$个随机变量序列，并且
 \begin{equation}
 \xi_{in}\overset{P}{\longrightarrow}a_i,\ n\to +\infty,\ \ (i=1,2,\cdots,k)
 \end{equation}
 又$R(x_1,x_2,\cdots,x_k)$是$k$元变量的有理函数，并且$R(a_1,a_2,\cdots,a_k)\neq \pm \infty$，则有
 \begin{equation}
 R(\xi_{1n},\xi_{2n},\cdots,\xi_{kn})\overset{P}{\longrightarrow}R(a_1,a_2,\cdots,a_k),\ \ n\to +\infty.
 \end{equation}

- **De Moivre-Laplace极限定理**：在$n$重Bernoulli试验中，事件$A$在每次试验中出现的概率是$p(0< p< 1)$，$\mu_n$是$n$次试验中$A$出现的次数，则
 \begin{equation}
 \lim_{n\to +\infty}P\Big{(}\frac{\mu_n-np}{\sqrt{npq}}\le x\Big{)}=\frac{1}{\sqrt{2\pi}}\int_{-\infty}^{x}e^{-\frac{t^2}{2}}dt.
 \end{equation}

- **Lindeberg-Levy定理**：若$\xi_1,\xi_2,\cdots$是一列独立同分布的随机变量，且
 \begin{equation}
 E\xi_k=a,D\xi_k=\sigma^2(\sigma^2>0),k=1,2,\cdots
 \end{equation}
 则有
 \begin{equation}
 \lim_{n\to +\infty}P\Big{(}\frac{\sum_{k=1}^{n}\xi_k-na}{\sigma\sqrt{n}}\le x\Big{)}=\frac{1}{\sqrt{2\pi}}\int_{-\infty}^{x}e^{-\frac{t^2}{2}}dt.
 \end{equation}

 \begin{equation}
 \end{equation}



## 二. 数理统计

### 1. 基本概念 
掌握数理统计的基本概念；熟练掌握矩估计法和极大似然估计法；熟练掌握无偏估计、有效估计和相合估计；熟练掌握区间估计定义及其意义。

- **母体**：研究对象的全体构成的集合称为母体或者总体，每一个成员称为个体。
- **样本**：假设抽取$n$个个体，且这$n$个个体的某一指标为$(\xi_1,\xi_2,\cdots,\xi_n)$，称这$n$个个体的指标$(\xi_1,\xi_2,\cdots,\xi_n)$为一个子样或者样本，$n$称为这个子样的容量。
- **抽样分布**：一个统计量是子样的一个函数，如果子样容量为$n$，它就是$n$个随机变量的函数，并且要求这个函数不依赖于任何未知参数的随机变量。统计量的分布称为抽样分布。
- **常用统计量**：设$\xi_1,\xi_2,\cdots,\xi_n$是从母体$\xi$中取出的容量为$n$的子样，统计量
 \begin{equation}
 \bar{\xi}=\frac{\sum_{i=1}^{n}\xi_i}{n}
 \end{equation}
 称为子样均值；统计量
 \begin{equation}
 S_{n}^2=\frac{1}{n}\sum_{i=1}^{n}(\xi_i-\bar{\xi})^2=\frac{1}{n}\sum_{i=1}^{n}\xi_i^2-\bar{\xi}^2
 \end{equation}
 称为子样方差；统计量
 \begin{equation}
 \bar{\xi^k}=\frac{1}{n}\sum_{i=1}^{n}\xi_i^k
 \end{equation}
 称为子样$k$阶矩；统计量
 \begin{equation}
 m_k=\frac{1}{n}\sum_{i=1}^n(\xi_i-\bar{\xi})^k
 \end{equation}
 称为子样$k$阶中心矩。

- **定理**：设母体$\xi$的分布函数$F(x)$具有二阶矩，即$E\xi=\mu< +\infty$,$D\xi=\sigma^2< +\infty$.若$\xi_1,\xi_2,\cdots,\xi_n$是取自这一母体的一个子样，则子样均值$\bar{\xi}$的数学期望与方差分别是
 \begin{equation}
 E\bar{\xi}=\mu,\ \ D\bar{\xi}=\frac{\sigma^2}{n}.
 \end{equation}
 假设母体的原点矩$\nu_k=E\xi^k$和中心矩$\mu_k=E(\xi-\nu_1)^k$,$k=1,2,3,4$都存在，则子样方差的数学期望和方差依次是
 \begin{equation}
 E(S_n^2)=\frac{n-1}{n}\mu_2,\ \ D(S_n^2)=\frac{\mu_4-\mu_2^2}{n}-\frac{2(\mu_4-2\mu_2^2)}{n^2}+\frac{\mu_4-3\mu_2^2}{n^3}.
 \end{equation}
 并且子样均值和子样方差的协方差为
 \begin{equation}
 Cov(\bar{\xi},S_n^2)=\frac{n-1}{n^2}\mu_3.
 \end{equation}
- **估计量**：设$\xi_1,\xi_2,\cdots,\xi_n$是取自母体的一个子样，构造一个统计量$\eta=u(\xi_1,\xi_2,\cdots,\xi_n)$作为参数$\theta$的估计，称统计量$\eta$为参数$\theta$的一个估计量。若$(x_1,x_2,\cdots,x_n)$是子样$(\xi_1,\xi_2,\cdots,\xi_n)$的一组观测值，则$y=u(x_1,x_2,\cdots,x_n)$就是$\theta$的一个点估计值简称点估计。   
 **点估计问题**：如果分布族中含有$k$个未知参数，即$\{f(x;\theta_1,\theta_2,\cdots,\theta_k):(\theta_1,\theta_2,\cdots,\theta_k)\in \Theta\}$，则需要构造$k$个统计量$\eta_1=u(\xi_1,\xi_2,\cdots,\xi_n),\cdots,\eta_k=u_k(\xi_1,\xi_2,\cdots,\xi_n)$分别作为$\theta_1,\theta_2,\cdots,\theta_k$的估计量，这种问题称为参数的点估计问题。
- **矩估计法**：设母体$\xi$具有已知类型的概率函数$f(x;\theta_1,\theta_2,\cdots,\theta_k)$，$(\theta_1,\theta_2,\cdots,\theta_k)\in \Theta$是$k$个未知参数。$\theta_1,\theta_2,\cdots,\theta_n$是取自母体$\xi$的一个子样。假设$\xi$的$k$阶矩$\nu_{k}=E\xi^k$存在，显然$\nu_j,j< k$都存在，并且是$\theta_1,\theta_2,\cdots,\theta_k$的函数$\nu_j(\theta_1,\theta_2,\cdots,\theta_k)$。子样$\xi_1,\xi_2,\cdots,\xi_n$的$j$阶矩为$\bar{\xi^j}=\frac{1}{n}\sum_{i=1}^{n}\xi_i^j$。设
 \begin{equation}
 \nu_j(\theta_1,\theta_2,\cdots,\theta_k)=\bar{\xi^j},\ \ j=1,2,\cdots,k
 \end{equation}
 得到含$k$个未知数$\theta_1,\theta_2,\cdots,\theta_k$的$k$个方程式。求解可得到$\theta_1,\theta_2,\cdots,\theta_k$的一组解：
 \begin{equation}
 \hat{\theta_i}=\hat{\theta_i}(\xi_1,\xi_2,\cdots,\xi_n),\ \ i=1,2,\cdots,k
 \end{equation}
 用$\hat{\theta_i}$估计$\theta_i$就是矩法估计。
- **相合估计**：设母体$\xi$具有概率函数$f(x,\theta)$,$\theta\in \Theta$为未知参数。$\hat{\theta}_ n=\hat{\theta}_ n(\xi_1,\xi_2,\cdots,\xi_n)$为$\theta$的一个估计量，$n$为样本容量。若对于任意$\varepsilon >0$，有
 \begin{equation}
 \lim_{n\to +\infty}P(\vert \hat{\theta}_ n-\theta\vert >\varepsilon)=0,
 \end{equation}
 则称$\hat{\theta}_ n$为参数$\theta$的相合估计。

- **无偏估计**：设$\hat{\theta}=\hat{\theta}(\xi_1,\xi_2,\cdots,\xi_n)$为母体$\xi$的概率函数$\{f(x;\theta):\theta\in \Theta\}$的未知参数$\theta$的一个估计量。若对于任意$\theta\in \Theta$有
 \begin{equation}
 E\big{(}\hat{\theta}(\xi_1,\xi_2,\cdots,\xi_n)\big{)}=\theta,
 \end{equation}
 则称$\hat{\theta}(\xi_1,\xi_2,\cdots,\xi_n)$为$\theta$的无偏估计，否则称为有偏的。   
 **渐近无偏估计**：如果$\theta$的一个估计$\hat{\theta}$不一定是无偏的，但是当$n\to +\infty$时，$E\hat{\theta}\to \theta$，则称$\hat{\theta}$为$\theta$的渐近无偏估计。

- **极大似然估计法**：设$\xi_1,\xi_2,\cdots,\xi_n$为取自具有概率函数$\{f(x;\theta):\theta\in \Theta\}$的母体$\xi$的一个子样。子样$\xi_1,\xi_2,\cdots,\xi_n$的联合概率函数在$\xi_i$取已知观测值$x_i$，$i=1,2,\cdots,n$时的值$f(x_1;\theta)f(x_2;\theta)\cdots f(x_n;\theta)$是$\theta$的函数。记
 \begin{equation}
 L(\theta)=L(\theta;x_1,x_2,\cdots,x_n)=f(x_1;\theta)f(x_2;\theta)\cdots f(x_n;\theta),
 \end{equation}
 称为这个子样的似然函数。  
 如果$\xi$是离散型母体，$L(\theta;x_1,x_2,\cdots,x_n)$给出观测到$(x_1,x_2,\cdots,x_n)$的概率。因此，可以把$L(\theta;x_1,x_2,\cdots,x_n)$看作观测到$(x_1,x_2,\cdots,x_n)$时出现什么样$\theta$的可能性的一个测度。寻找观测值$(x_1,x_2,\cdots,x_n)$的函数$\hat{\theta}=\hat{\theta}(x_1,x_2,\cdots,x_n)$，用$\hat{\theta}$代替$\theta$使得
 \begin{equation}
 L(\hat{\theta};x_1,x_2,\cdots,x_n)=\sup_{\theta\in \Theta}L(\theta;x_1,x_2,\cdots,x_n),
 \end{equation}
 满足上式的$\hat{\theta}(x_1,x_2,\cdots,x_n)$就是可能产生$x_1,x_2,\cdots,x_n$的参数$\theta$的值。称$\hat{\theta}(x_1,x_2,\cdots,x_n)$为参数$\theta$的极大似然估计值，相应的估计量$\hat{\theta}(\xi_1,\xi_2,\cdots,\xi_n)$称为参数$\theta$的极大似然估计量。  
 如果$\xi$是连续型，$f(x;\theta),\theta\in \Theta$表示密度函数。于是子样$(\xi_1,\xi_2,\cdots,\xi_n)$落入点$(x_1,x_2,\cdots,x_n)$的邻域内的概率是$\prod_{i=1}^{n}f(x_i;\theta)\delta x_i$，同样是$\theta$函数。既然$(x_1,x_2,\cdots,x_n)$在一次抽烟中出现，便认为子样$(\xi-1，\xi_2,\cdots,\xi_n)$落在落在$(x_1,x_2,\cdots,x_n)$的邻域内的概率达到最大。所有找到使得$\prod_{i=1}^{n}f(x_i,\theta)\Delta x_i$达到最大的$\theta$的值$\hat{\theta}(x_1,x_2,\cdots,x_n)$。由于$\Delta x_i$是不依赖于$\theta$的增量，只需要求出使得
 \begin{equation}
 L(\theta;x_1,x_2,\cdots,x_n)=\prod_{i=1}^{n}f(x_i;\theta)
 \end{equation}
 达到极大的$\hat{\theta}(x_1,x_2,\cdots,x_n)$，便可得到极大似然估计。   
 **方法**：
 1. 写出极大似然函数；
 2. 求出极大似然函数的极值点，便为估计量。   
 **性质**：设$\hat{\theta}$为$f(x;\theta)$的参数$\theta$的极大似然估计，并且函数$u=u(\theta)$具有单值反函数$\theta=\theta(u)$，则$\hat{u}=u(\hat{\theta})$是$u(\theta)$的极大似然估计，其中$\theta\in \Theta$，记$U$为$u(\theta)$的值域。

- **有效**：设参数$\theta$有两个无偏估计$\hat{\theta_1}$和$\hat{\theta_2}$，他们的方差对于任意的$\theta\in \Theta$有$D(\hat{\theta_1})\le D(\hat{\theta})$，则称估计$\hat{\theta_1}$比$\hat{\theta_2}$有效。
- **有效估计**：若$\theta$的一个无偏估计$\hat{\theta}$使等式
 \begin{equation}
 D(\hat{\theta})=\frac{1}{nE\big{(}\frac{\partial}{\partial \theta}\ln{f(\xi;\theta)}\big{)}^2}
 \end{equation}
 成立，则称$\hat{\theta}$是$\theta$的有效估计。
- **有效率**：如果$\hat{\theta_1}$是$\theta$的无偏估计，则称
 \begin{equation}
 e=\frac{1/(nI(\theta))}{D(\hat{\theta_1})}
 \end{equation}
 为估计$\hat{\theta_1}$的有效率，其中$I(\theta)=E\big{(}\frac{\partial}{\partial \theta}\ln{f(\xi;\theta)}\big{)}^2$.
- **渐近有效估计**：当$n\to \infty$时，一个估计量$\hat{\theta}$的有效率$e\to 1$，则称$\hat{\theta}$为参数$\theta$的渐近有效估计。


### 2.假设检验 
充分理解和掌握 Neyman-Pearson 假设检验的基本思想和方法；熟练掌握正态总体参数假设检验方法。

- **假设**：吧一个有未知分布的假设称为统计假设或者假设。
- **参数假设**：涉及到母体分布的未知参数的统计假设称为参数假设。  
 **分参数假设**：统计假设只能对未知分布函数的类型或者它的某种特征提出某种假设，称为非参数假设。
- **简单统计假设**：如果一个统计假设完全确定母体分布，则称此假设为简单统计假设，否则称为符合统计假设或复合假设。
- **检验**：再对$H_0$对$H_1$的检验问题中，从子样$(\xi_1,\xi_2,\cdots,\xi_n)$出发，制定一个法则，通过确定的$(x_1,x_2,\cdots,x_n)$判断拒绝$H_0$还是$H_1$，这种法则称为$H_0$对$H_1$的一个检验法则，简称检验法则或检验。
- **拒绝域**：检验法则将子样空间划分为两个不相交的子集$C$和$C^{* }$，如果$(x_1,x_2,\cdots,x_n)\in C$，则拒绝$H_0$，否则拒绝$H_1$接受$H_0$，称子样空间$C$为临界域或拒绝域。

- **第一类错误**：当$H_0$为真时，子样的观测值落入拒绝域$C$，则应当拒绝$H_0$，这种错误称为第一类错误，其发生概率称为犯第一类错误的概率或者拒真概率，记作$\alpha$，即
 \begin{equation}
 P(\text{拒绝}H_0 \vert H_0 \text{为真})=\alpha.
 \end{equation}
- **第二类错误**：当$H_1$为真时，而子样的观测值落入$C^{* }$($C$的补集)，则应当接受$H_0$，这种错误称为第二类错误，发生的概率称为犯第二类错误的概率或受伪概率，记作$\beta$，即
 \begin{equation}
 P(\text{接受}H_0\vert H_1\text{为真})=\beta.
 \end{equation}

- **正态母体的参数假设检验**：
 1. **$u$检验**：设$\xi_1,\xi_2,\cdots,\xi_n$是取自正态母体$N(\mu,\sigma^2)$的一个子样，$\sigma^2=\sigma_0^2$为已知常数，要检验假设$H_0:\mu=\mu_0$，$H_1:\mu\neq \mu_0$。首先通过$N(0,1)$计算$1-\frac{\alpha}{2}$的分位点$u_{1-\frac{\alpha}{2}}$，确定拒绝域$C=(\vert u\vert \ge u_{1-\frac{\alpha}{2}})$，其中$u=\frac{\bar{\xi}-\mu_0}{\sigma_0/\sqrt{n}}$，得到检验结果。
 2. **$t$检验**：设$\xi_1,\xi_2,\cdots,\xi_n$是取自正态母体$N(\mu,\sigma^2)$的一个子样，$\sigma^2$为未知常数，要检验假设$H_0:\mu=\mu_0$，$H_1:\mu\neq \mu_0$。首先通过自由度为$(n-1)$的$t$分布计算$t_{1-\frac{\alpha}{2}}(n-1)$，确定拒绝域$C=(\vert t\vert \ge t_{1-\frac{\alpha}{2}}(n-1))$，其中$t=\frac{\bar{\xi}-\mu_0}{S_n^{* }}\sqrt{n}$.
 3. **$\chi^2$检验**：设$\xi_1,\xi_2,\cdots,\xi_n$是取自正态母体$N(\mu,\sigma^2)$的一个子样，要检验假设$H_0:\sigma^2=\sigma_0^2$，$H_1:\sigma^2\neq \sigma_0^2$。(a) $\mu=\mu_0$为已知常数，通过自由度为$n$的$\chi^2$分布计算$\frac{\alpha}{2}$和$1-\frac{\alpha}{2}$的分位点$k_1=\chi_{\frac{\alpha}{2}}^2(n)$和$k_2=\chi_{1-\frac{\alpha}{2}}^2(n)$，确定拒绝域$C=(\chi^2<\chi_{\frac{\alpha}{2}}^2(n))\bigcup (\chi^2> \chi_{1-\frac{\alpha}{2}}^2(n))$，其中$\chi^2=\frac{\sum_{i=1}^n(\xi_i-\mu_0)^2}{\sigma_0^2}$。(b) $\mu$是未知数，$\chi^2=\frac{\sum_{i=1}^n(\xi_i-\bar{\xi})^2}{\sigma_0^2}$，其他类似(a)的拒绝域。
 4. **$F$检验**：设$\xi_1,\xi_2,\cdots,\xi_{n_1}$是取自正态母体$N(\mu_1,\sigma_1^2)$的一个子样，$\eta_1,\eta_2,\cdots,\eta_{n_2}$是取自正态母体$N(\mu_2,\sigma_2^2)$的一个子样，要检验假设$H_0:\sigma_1^2=\sigma_2^2$，$H_1:\sigma_1^2\neq \sigma_2^2$。通过自由度为$n_1-1,n_2-1$的$F$分布计算$F_{1-\frac{\alpha}{2}}(n_1-1,n_2-1)$和$F_{\frac{\alpha}{2}}(n_1-1,n_2-1)$，确定拒绝域$C=\big{(}F\le F_{\frac{\alpha}{2}}(n_1-1,n_2-1)\big{)}\bigcup \big{(}F\ge F_{1-\frac{\alpha}{2}}(n_1-1,n_2-1)\big{)}$，其中$F=\frac{S_{1n_1}^{* 2}}{S_{2n_2}^{* 2}}$。

- **置信区间**：设母体$\xi$具有概率密度函数$f(x;\theta)$，$\theta$为未知参数。$\xi_1,\xi_2,\cdots,\xi_n$为取自母体$\xi$的子样。若对于给定的$\alpha$($0< \alpha< 1$)，存在两个统计量$\underline{\theta}(\xi_1,\xi_2,\cdots,\xi_n)$和$\bar{\theta}(\xi_1,\xi_2,\cdots,\xi_n)$使得
 \begin{equation}
 P(\underline{\theta}(\xi_1,\xi_2,\cdots,\xi_n)< \theta <\bar{\theta}(\xi_1,\xi_2,\cdots,\xi_n))=1-\alpha,
 \end{equation}
 则称区间$(\underline{\theta},\bar{\theta})$为参数$\theta$的置信度为$1-\alpha$的置信区间，$\underline{\theta}$和$\bar{\theta}$分别称为置信度$1-\alpha$的置信下限和置信上限。   
 **寻找步骤**：
 1. 寻找子样$(\xi_1,\xi_2,\cdots,\xi_n)$的一个函数$u(\xi_1,\cdots,\xi_n;\theta)$，满足$u$除了$\theta$之外不含其他未知参数，且其分布不含未知参数。
 2. 对于给定的置信度$1-\alpha$确定分位点。
 3. 利用不等式变形求得未知数$\theta$的置信区间。

<!-- - **正态母体的参数置信区间**：

- **Neyman-Pearson 假设检验**：

- **区间估计**：

 \begin{equation}
 \end{equation} -->
