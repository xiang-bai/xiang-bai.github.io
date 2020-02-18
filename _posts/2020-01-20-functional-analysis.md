---
layout: post
title:  "泛函分析基础"
date:   2020-01-20 02:34:20 +0800
categories: math
tags: analysis
---

# 泛函分析基础

## 介绍

- 本文围绕Rudin的教材来学习泛函分析。

## 拓扑向量空间

### 简介

#### 赋范空间

- **赋范空间**：如果在向量空间$X$上对于任意$x\in X$存在非负实数$\|x\|$，满足  
(1) $\|x+y\| \le \|x\| +\|y\|$, $\forall x,y \in X$;  
(2) $\|\alpha x\| = |\alpha| \|x\|$, $x \in X$, $\alpha$为标量;  
(3) $\|x\| > 0$, $x\neq 0$;  
则称$X$为赋范向量空间，$\|x\|$称为$x$的范数。

- **赋范空间$\to$距离空间**：每一个赋范向量空间可以诱导一个距离空间($d(x,y)=\|x-y\|$)。
- **开球和闭球**：球心为$x$半径为$r$的开球和闭球分别是
\begin{equation}
B_{r}(x)=\{y:d(x,y)< r \},\ \ \bar{B} _ {r}(x)=\{y:d(x,y)\le r \}.
\end{equation}

- **开集**：距离空间上的子集是开集当且仅当它是一些开球的并，进而可以所有这样的子集构成一个拓扑。如果距离是赋范空间诱导得到，那么在这个拓扑上，向量的加法和数乘连续。

- **Banach空间**：完备的赋范空间（在诱导的距离上，Cauchy列收敛）。

#### 向量空间

- **向量空间**：数域$\Phi$上的集合$X$，定义加法和数乘满足：  
(1) $a+b=b+a$, 对任意$a,b\in X$;  
(2) $a+(b+c)=(a+b)+c$, 对任意$a,b,c\in X$;  
(3) 存在一个元素$0\in X$, 对一切$a\in X$有$a+0=a$，元素$0$称为$X$的零元;  
(4) 对任意$a\in X$, 都存在$b\in X$使$a+b =0$，$b$称为$a$的负元素，记为$-a$;  
(5) 对$\Phi$中单位元$1$，有$1a=a$$(a\in X)$;  
(6) 对任意$\alpha, \beta \in \Phi$, $a\in X$有$(\alpha\beta)a=\alpha(\beta a)$;   
(7) 对任意$\alpha, \beta \in \Phi$, $a\in X$有$(\alpha+\beta)a=\alpha a +\beta a$;   
(8) 对任意$\alpha\in \Phi$, $a,b\in X$有$\alpha (a+b)=\alpha a+\alpha b$;
称$X$为向量空间。  

- **子空间**：如果$Y\subset X$, 且$Y$也是向量空间，称$Y$为$X$子空间。
- **子空间等价命题**：$Y$为向量空间$X$的子空间等价于任意标量$\alpha,\beta$有
\begin{equation}
\alpha Y +\beta Y\subset Y.
\end{equation}


- **凸的**：如果向量空间$X$的子集$C\subset X$，满足
\begin{equation}
tC + (1-t)C\subset C, \ \ \  (0\le t\le 1),
\end{equation}
称$C$为凸的。
- **均衡的**：如果向量空间$X$的子集$B\subset X$，满足
\begin{equation}
\alpha B\subset B, \ \ \ \forall \alpha \in \Phi(|\alpha |\le 1),
\end{equation}
称$B$为均衡的。
- **维数**：如果向量空间$X$有一组基$\{u_1,u_2,\cdots,u_n\}$，则称$X$为$n$维的。


#### 拓扑空间

- **拓扑空间**：对于集合$S$, 设$\tau$为$S$的子集族(每个元素叫做一个开集)满足，  
(1) $S$是开集，$\varnothing$是开集；  
(2) 任意两个开集的交集还是开集；  
(3) 任意开集族的并还是开集；  
称$(S,\tau)$为拓扑空间，$\tau$是$S$的拓扑。
- **闭的**：集合$E\subset S$是闭的等价于它的补集是开的。
- **闭包**：$E$的闭包$\bar{E}$是所有包含$E$的闭集的交集。
- **内部**：$E$的内部$E^{\circ}$是$E$的所有开子集的并集。
- **邻域**：点$p\in S$的邻域是任意包含$p$的开集。
- **Hausdorff空间**：如果$S$上不同的点有不相交的领域，称$(S,\tau)$是Hausdorff空间，$\tau$是Hausdorff拓扑。
- **紧的**：如果集合$K\subset S$的任意一个开覆盖都有有限子覆盖，称$K$是紧的。(注意任意性。)
- **基**：对于一个族$\tau'\subset \tau$，如果$\tau$上的元素都是$\tau'$中元素的并集，则称$\tau'$为$\tau$的一个基。
- **局部基**：对于点$p$的邻域族$\gamma$，如果$p$的任意邻域都包含$\gamma$的元素，则称$\gamma$为$p$点的局部基。
- **拓扑继承**：如果$E\subset S$，并且$\sigma$是所有$E\cap V$($V\in \tau$)组成的族，则$\sigma$是$E$的拓扑，称为$E$继承于$S$的拓扑。
- **相容**：如果拓扑$\tau$由距离$d$诱导得到，则称$\tau$与$d$相容。
- **收敛**：对于Hausdorff空间上的序列$\{x_n\}$, 如果点$x\in X$的每一个邻域都包含序列中除了有限个$x_n$外的所有，则称$x_n$收敛到$x$(记作$\lim \limits_ {n\to \infty} x_n = x$).

#### 拓扑向量空间

- **拓扑向量空间**：假设$\tau$是向量空间$X$上的拓扑，满足  
(1) $X$的每一个点是闭集；   
(2) 向量空间的运算关于$\tau$连续；  
则称$\tau$是$X$的向量拓扑，$X$是一个拓扑向量空间。  
 **注**：(连续的意义)关于加法连续是指从$X\times X$到$X$的映射：$(x,y)\to x+y$是连续的，即如果$x_1,x_2\in X$, $V$是$x_1+x_2$的邻域，则存在$x_1$和$x_2$的邻域$V_1$和$V_2$满足
 \begin{equation}
 V_1+V_2\subset V.
 \end{equation}
 类似乘法的连续是$\Phi \times X$到$X$的映射：$(\alpha, x)\to \alpha x$是连续的。即，如果$x\in X$，$\alpha$是标量，$V$是$\alpha x$的邻域，则存在某个$r>0$和$x$的某个邻域$W$满足任意的$|\beta-\alpha|< r $有$\beta W\subset V$.
- **有界**：对于拓扑向量空间$X$的子集$E$, 如果$0$的任意邻域$V$都存在$s>0$满足任意$t>s$有$E\subset tV$.

#### 不变性

- **同胚**：两个拓扑空间$(X,\tau_X)$和$(Y,\tau_Y)$之间的映射$f:X\to Y$称为同胚，如果它具有下列性质：  
(1) $f$是双射（既是单射又是满射）；  
(2) $f$是连续的；  
(3) $f$的逆映射也是连续的（f是开映射）。
- **同胚映射$T_a$和$M_{\lambda}$**：对于每一个$a\in X$和标量$\lambda$，定义平移算子$T_a$和乘算子$M_{\lambda}$如下，
$$T_a(x) = a+x,\ \ \ M_{\lambda}(x)=\lambda x,\ \ \ (x\in X)$$
则$T_a$和$M_{\lambda}$为同胚映射。   
证明：验证3条。
- **向量拓扑是平移不变的**：向量拓扑是平移不变的(简称为不变)：集合$E\subset X$是开集等价于它的每一个平移变换$a+E$是开的。因此$\tau$完全由任意的局部基决定。
- **局部基**：在拓扑向量空间下，局部基将总是指$0$点的局部基。因此，拓扑向量空间$X$的局部基是$0$的一个邻域族$\mathcal{B}$，每一个邻域为$\mathcal{B}$的一个元素。于是$X$的开集是$\mathcal{B}$中一些元素的并集。
- **距离不变性**：向量空间$X$的距离$d$被称为不变的，如果对于任意的$x,y,z\in X$有
\begin{equation}
d(x+z,y+z)=d(x,y).
\end{equation}


#### 拓扑向量空间的类型

### 分离性质
- **定理**：假设$K,C$是拓扑向量空间$X$的子集，$K$是紧集，$C$是闭集，且$K\cap C= \varnothing$. 则存在$0$的邻域$V$满足   
 \begin{equation}
 (K+V)\cap (C+V)=\varnothing.
 \end{equation}
 **注**： 注意$K+V$是所有$x+V$的并集$x\in K$，因此$K+V$是包含$K$的开集。因此，定理意味存在包含$K$和$C$的互不相交的开集。  
 **证明**：先介绍如下命题，在$X$中如果$W$是$0$的一个邻域，则存在$0$的对称邻域$U$(即$U=-U$)满足，$U+U\subset W$。 
 先证明上述命题，注意到$0+0=0$，由加法的连续性，存在$0$的邻域$V_1,V_2$满足$V_1+V_2\subset W$. 如果取    
 \begin{equation}
 U=V_1\cap V_2\cap (-V_1)\cap (-V_2),
 \end{equation}
 则$U$满足上述命题的要求。
 在上述命题中，$U$可以视作一个$W$，故存在$0$的对称邻域$U$满足   
 \begin{equation}
 U+U+U+U\subset W.
 \end{equation}
 明显可以一直这样做下去。  
 如果$K=\varnothing$，则$K+V=\varnothing$，故定理的结论明显。
 下面考虑$K\neq \varnothing$，一个点$x\in K$。
 由于$C$是闭集，故$C$的补集$X-C$是开集，又$x\notin C$有$x\in X-C$，再由拓扑的平移不变性和上述命题有，存在$0$的对称邻域满足  
 \begin{equation}
 x+V_x+V_x+V_x\subset X-C,
 \end{equation}
 即$x+V_x+V_x+V_x$与$C$不相交，再由$V_x$的对称性有  
 \begin{equation}
 (x+V_x+V_x)\cap (C+V_x)=\varnothing,
 \end{equation}
 由于$K$是紧集，故存在$x_1,x_2,\cdots,x_n \in K$，满足  
 \begin{equation}
 K\subset (x_1+V_{x_1})\cup \cdots \cup (x_n+V_{x_n}),
 \end{equation}
 取$V=V_{x_1}\cap \cdots \cap V_{x_n}$. 则  
 \begin{equation}
 K+V \subset \bigcup\limits_{i=1}^{n}(x_i+V_{x_i}+V) \subset x_i+V_{x_i}+V_{x_i},
 \end{equation}
 而又有$C+V \subset C+V_{x_i}$，结合前面的公式有  
 \begin{equation}
 (K+V) \cap (C+V) =\varnothing.
 \end{equation}
 证明完成。$\blacksquare$ 

- **定理**：如果$\mathcal{B}$是拓扑向量空间$X$的局部基，则任意的$S\in \mathcal{B}$，存在$E\in \mathcal{B}$满足，$E$的闭包$\bar{E}$包含于$S$。   
 **证明**：由于$S$为开集，故它的补集$S^{c}$为闭集，去$K=\{x\}(x\in S)$，则$S\cap K=\varnothing$. 又$K$为紧集，故存在$0$的邻域$V$满足， 
 \begin{equation}
 (K+V)\cap (S^c+V)=\varnothing.
 \end{equation}
 又因为$S^c+V$是开集，故$K+V=x+V$的闭包也与$S^c+V$不相交。而$x+V$是开集，故存在$\mathcal{B}$中元素$E$包含于$x+V$，明显有  
 \begin{equation}
 \bar{E}\subset \overline{x+V}\subset S.
 \end{equation}
 证明完毕。$\blacksquare$

- **定理**：每一个拓扑向量空间是一个Hausdorff空间。   
 **证明**：任意取空间上的两个点明显可视作一个是紧集，一个是闭集，故两个点存在不相交的邻域。$\blacksquare$

- **闭包等价刻画**：对于拓扑空间$X$，$E$是$X$上的子集，则$ p\in \bar{E}$等价于$p$的任意邻域都与$E$相交。  
 **证明**： 如果$p\in E$明显$p$的任意邻域都与$E$相交，下面考虑$p\notin E$，设$S$为$p$的邻域，则$S$的补集$S^c$为闭集，而$x\notin S^c$故$E\nsubseteq S^c$，故$S\cap E \neq \varnothing$。再证反方向，如果$p$的任意邻域都与$E$相交，假设存在闭集$S$满足$E\subset S$，且$p\notin S$，故$p\in S^c$，又$S^c$为开集，故$S^c \cap E \neq \varnothing$，产生矛盾，证明完毕。$\blacksquare$

- **定理**：设$X$是拓扑向量空间，则  
 (a). 如果$A\subset X$，则$\bar{A}=\bigcap (A+V)$，交集中$V$跑遍所有$0$的邻域。  
 (b). 如果$A\subset X$且$B\subset X$，则$\bar{A}+\bar{B}\subset \overline{A+B}$。  
 (c). 如果$Y$是$X$的子空间，则$\bar{Y}$也是。  
 (d). 如果$C$是$X$上的凸子集，则$\bar{C}$和$C^{\circ}$也是。  
 (e). 如果$B$是均衡子集，则$\bar{B}$也是，如果额外有$0\in B^{\circ}$，有$B^{\circ}$也是均衡的。  
 (f). 如果$E$是有界子集，则$\bar{E}$也是。  
 **证明**：  
 (a). $x\in \bar{A}$等价于所有$0$的邻域$V$，$(x+V)\cap A\neq \varnothing $，进而等价于所有$0$的邻域$V$，$x\in (A-V) $.  
 (b). 任取$a\in A， b\in B$，对于$a+b$的邻域$W$，由连续性存在$a$的邻域$W_1$，$b$的邻域$W_2$，满足$W_1 +W_2 \subset W$，又因为$W_1\cap A\neq \varnothing$, $W_2 \cap B\neq \varnothing$，则$W\cap (A+B)\neq \varnothing$，故$a+b\in \overline{A+B}$.   
 (c). 假设$\alpha,\beta$是两个标量，则$\alpha \bar{Y}=\overline{\alpha Y}$，故  
 $$\alpha \bar{Y}+\beta \bar{Y}=\overline{\alpha Y}+\overline{\beta Y}\subset \overline{\alpha Y+\beta Y}\subset \bar{Y}.$$     
 对于凸子集的闭包也是凸子集和均衡集的闭包也是均衡集的证明类似，下面省略。  
 (d). 如果$0< t < 1$，有
 $$tC^{\circ}+(1-t)C^{\circ}\subset C.$$
 因为左边的两个集合是开集，故他们的和也是开集。又$C$的每一个开集都是$C^{\circ}$的子集，故$C^{\circ}$是凸的。  
 (e). 如果$0<|\alpha|\le 1$，由于$x \to \alpha x$是同胚映射，有$\alpha B^{\circ} = (\alpha B)^{\circ}$，进而再由均衡性有$\alpha B^{\circ} \subset \alpha B \subset B$。而$\alpha B$是开集，故$\alpha B^{\circ} \subset B^{\circ}$。如果$0\in B^{\circ}$，故$\alpha = 0$时也有$\alpha B^{\circ} \subset B^{\circ}$。因此，$B^{\circ}$是均衡的。  
 (f). 设$V$是$0$的邻域，则存在$0$的邻域$W$满足$\bar{W}\subset V$。又$E$ 有界，故存在$t>0$满足$E\subset tW$，进而$\bar{E}\subset t\bar{W} \subset tV$。
 证明完毕。$\blacksquare$


- **定理**：再拓扑向量空间$X$中，  
 (a). $0$的每一个邻域包含一个$0$的均衡邻域；  
 (b). $0$的每一个凸邻域包含一个$0$的均衡凸邻域。   
 **证明**：
 (a). 设$U$是$0$的邻域，则由数乘的连续性，存在实数$\delta>0$和$0$的邻域$V$满足任意的$\vert \alpha \vert<\delta$有$\alpha V\subset U$。取$W=\bigcup\limits_{\vert \alpha\vert <\delta}\alpha V$，则对于任意的$\vert \beta\vert<1$有，$\beta W=\bigcup\limits_{\vert \alpha\vert <\delta}(\alpha \beta)V=\bigcup\limits_{\vert \alpha\vert <\delta\beta}\alpha V\subset W$，而又明显$W$是$0$的邻域，因此$W$均衡的。   
 (b). 假设$U$是$0$在$X$的凸邻域，取$A=\bigcap\limits_{\vert \alpha \vert=1}\alpha U$，如(a)中选取集合$W$，由于$W$是均衡的，故对于$\vert \alpha\vert=1$有$\alpha^{-1}W=W$，因此$W\subset \alpha U$。进而有$W\subset A$，故$A$的内部$A^{\circ}$是$0$的一个邻域。由于$U$是凸集，故$A$是凸集的交集，故$A$也是凸集，因此$A^{\circ}$是凸集。对于任意的$0\le r\le 1$和$\vert \beta \vert=1$有
 \begin{equation}
 r\beta A=\bigcap\limits_{\vert \alpha \vert=1}r\beta\alpha U= \bigcap\limits_{\vert \alpha \vert=1}r\alpha U.
 \end{equation}
 由于$\alpha U$是一个包含$0$的凸集，故$r\alpha U\subset \alpha U$，因此$r\beta A\subset A$，即$A$是均衡集，进而$A^{\circ}$是均衡集。
 证明完毕。$\blacksquare$  
 **均衡局部基和凸局部基**：如果局部基的每一个元素都是均衡集，称其是均衡局部基，如果局部基的每一个元素都是凸集，则称其是凸局部基。   
 **推理**：  
 (a). 每一个拓扑向量空间有一个均衡的局部基。  
 (b). 每一个局部凸空间有一个均衡的凸局部基。

- **定理**：在拓扑向量空间$X$中，设$V$是$0$的邻域，  
 (a). 如果$0< r_1 < r_2 <\cdots $满足当$n\to \infty$，$r_n\to \infty$，则
 $$X=\bigcup\limits_{n=1}^{\infty}r_n V.$$  
 (b). $X$的每一个紧子集$K$是有界的。  
 (c). 如果$\delta_1>\delta_2>\cdots$满足当$n\to \infty$时$\delta_n\to 0$，且$V$有界，则族$ \{ \delta_n V :n=1,2,\cdots \}$是$X$的局部基。  
 **证明**：(a). 对于任意$x\in X$，由于映射$0x$连续，对于$0x$的邻域$V$，存在$\delta>0$和$x$的某个邻域$W$，满足当$\vert \alpha-0\vert\le \delta$时，$\alpha W\subset V$。又$r_n\to \infty$故，充分大的$n$时有$\vert 1/r_n\vert\le \delta$，因此$1/r_n x\in 1/r_n W\subset V$，即$x\in r_n V$。   
 (b). 对于任意$0$的邻域$V$，存在$0$的均衡邻域$W$满足$W\subset V$。在通过(a)有$W\subset \bigcup\limits_{n=1}^{\infty}nW$。再由紧性，存在有限个正整数$n_1< n_2< \cdots< n_s$满足$K\subset n_1W\cup\cdots\cup n_s W\subset n_s W$，其中最后一个包含用到了均衡性。因此，如果$t>n_s$，则有$k\subset t W\subset tV$。  
 (c). 设$U$是$X$上$0$的一个邻域，由于$V$有界，则存在$s>0$，当$t>s$有$V\subset tU$，又$\delta_n\to 0$，有充分大的$n$时$1/\delta_n>s$，因此$V\subset 1/\delta_n U$，即$\delta_n V\subset U$。
 证明完毕。$\blacksquare$





### 线性映射

### 有限维空间

### 度量化

### 有界和连续

### 半范数和局部凸性

### 商空间

### 例子

### 习题

<!--  

## 完备性

### Baire纲

### Banach-Steinhaus定理

### 开映射定理

### 闭图像定理

### 双线性映射

### 习题




## 凸性

### Hahn-Banach 定理

### 弱拓扑

### 紧凸集

### 向量值积分

### 全纯函数

### 习题



## Banach空间的对偶

### 赋范空间的赋范对偶

### 伴随

### 紧算子

### 习题



## 一些应用

### 一个连续定理

### $L^{p}$空间的闭子空间

### 向量值测度的范围

### 一般的Stone-Weierstrass 定理

### 两个插值定理

### Kakutani不动点定理

### 紧群上的Haar测度

### 不可余子空间

### Poisson核的和

### 另两个不动点定理

### 习题

-->

