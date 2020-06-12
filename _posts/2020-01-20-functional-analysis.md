---
layout: post
title:  "泛函分析基础"
date:   2020-01-20 02:34:20 +0800
categories: math
tags: analysis
---

# 泛函分析基础

* any list
{:toc}

## 0 介绍

- 本文围绕Rudin的教材来学习泛函分析。

### 0.1 重要名词

- **紧**：给定拓扑空间$S$，如果集合$K\subset S$的任意一个开覆盖都有有限子覆盖，则称$K$是紧的。(注意任意性。)
- **稠密**：给定拓扑空间$S$及其子集$E$，对于$S$中任一点$x$，如果$x$的任一邻域与$E$的交集非空，则称$E$在$S$中稠密。
- **有界**：
- **Heine-Borel性质**：如果$X$的每一个有界闭子集都是紧集，则称其满足Heine-Borel性质。

- **F空间**：如果拓扑空间的拓扑由一个完备不变距离诱导得到，称其为拓扑空间。
- **Hausdorff空间**：对于拓扑空间$(S,\tau)$，如果$S$上不同的点有不相交的领域，称$(S,\tau)$是Hausdorff空间，$\tau$是Hausdorff拓扑。

- **局部凸**：如果$X$存在局部基它的每一个元素是凸的，则称$X$局部凸。

## 1 拓扑向量空间

### 1.1 简介

#### 1.1.1 赋范空间

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

#### 1.1.2 向量空间

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


#### 1.1.3 拓扑空间

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

#### 1.1.4 拓扑向量空间

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

#### 1.1.5 不变性

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


#### 1.1.6 拓扑向量空间的类型

$X$拓扑向量空间，对应拓扑是$\tau$，
- **局部凸**：如果$X$存在局部基，并且局部基的每一元都是凸的。
- **局部有界**：如果$0$存在有界邻域。
- **局部紧**：如果$0$有个邻域，其闭包是紧的。
- **可度量化**：如果$\tau$与某个度量$d$相容。
- **F-空间**：如果$\tau$由一个完备不变度量诱导得到。
- **Fréchet空间**：如果$X$是局部凸的F-空间。
- **可赋范的**：如果在$X$上存在范数满足诱导的度量与拓扑$\tau$相容。
- **Heine-Borel性质**：如果$X$的每一有界闭子集是紧的。

### 1.2 分离性质
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


### 1.3 线性映射

- **像和原像**：设$f$是点集$X$到$Y$的映射，如果$A\subset X$，$B\subset Y$,则$A$的像$f(A)$和$B$的原像或者逆像$f^{-1}(B)$是
 \begin{equation}
 f(A)=\{f(x):x\in A\},\ \ f^{-1}(B)=\{x:f(x)\in B\}.
 \end{equation}

- **线性**：设$X$和$Y$是同一标量域上的向量空间，如果对于任意$x,y\in X$和任意标量$\alpha,\beta$，映射$\Lambda: X\to Y$满足
 \begin{equation}
 \Lambda(\alpha x+\beta y)=\alpha \Lambda x+\beta \Lambda y.
 \end{equation}
 **线性泛函**：由$X$到标量域的线性映射称为线性泛函。

- **定理**：设$X$和$Y$是拓扑向量空间，如果$\Lambda:X\to Y$是线性的且在$0$点连续，则$\Lambda$连续。事实上，在下述意义$\Lambda$一致连续：对于$Y$中每个$0$的邻域$W$，存在$X$上的$0$点邻域$V$满足任意$x,y\in X$,
 \begin{equation}
 y-x\in V \Rightarrow \Lambda y-\Lambda x\in W.
 \end{equation}

- **定理**：设$\Lambda$是拓扑向量空间$X$上的线性泛函，如果存在$x\in X$满足$\Lambda x\neq 0$，则如下四个命题等价：
 1. $\Lambda$是连续的。
 2. 空间的核$\mathcal{N}(\Lambda)$是闭的。
 3. $\mathcal{N}(\Lambda)$在$X$中不稠密。
 4. 存在$0$的邻域满足$\Lambda$有界。

### 1.4 有限维空间

- **引理**：如果$X$是复的拓扑向量空间，且$f:\mathbb{C}^{n}\to X$是线性的，则$f$连续。
- **定理**：如果$n\in \mathbb{Z}^{+}$且$Y$是复拓扑向量空间$X$的$n$维子空间，则任意$\mathbb{C}^{n}$到$Y$的同构映射是同胚的并且$Y$是闭的。
- **定理**：所有局部凸拓扑向量空间都是有限维的。
- **定理**：如果局部有界拓扑向量空间满足Heine-Borel性质，则$X$是有限维的。
\begin{equation}
 \end{equation}

### 1.5 度量化

- **可度量的**：对于集合$X$上的拓扑$\tau$，如果存在度量$d$与$\tau$相容，则称$\tau$为可度量的。

- **定理**：如果拓扑向量空间$X$具有可数局部基，则$X$上存在度量$d$满足
 1. $d$与$X$的拓扑相容。
 2. 中心在$0$的开球是均衡的。
 3. $d$是不变的，即任意$x,y,x\in X$有，
 \begin{equation}
 d(x+z,y+z)=d(x,y).
 \end{equation}
 此外，如果$X$是局部凸的，则还有
 4. 所有开球是凸的。
- **Cauchy列**：设$\tau$是拓扑向量空间$X$的拓扑，$\mathcal{B}$是$\tau$的一个局部基，对于$X$上的点列$\{x_n\}$，如果任意$V\in \mathcal{B}$，存在$N$使得$m,n>N$有$x_m-x_n\in V$，则称$\{x_n\}$为Cauchy列。

- **膨胀原理**：设$(X,d_1)$，$(Y,d_2)$是度量空间，其中$(X,d_1)$是完备的。如果$E$是$X$中的闭集，$f:E\to Y$连续，并且任意$x',x''\in E$有
 \begin{equation}
 d_2\big{(}f(x'),f(x'')\big{)}\ge d_1(x',x''),
 \end{equation}
 则$f(E)$是闭的。

- **定理**：设$Y$是拓扑向量空间$X$的子空间，且$Y$是($X$诱导的拓扑下的)F空间($X$诱导的拓扑)。则$Y$是$X$的闭子空间。

- **定理**：
 1. 如果$d$是向量空间$X$上的平移不变度量，则对于任意的$x\in X$和$n=1,2,3,\cdots$有
 \begin{equation}
 d(nx,0)\le nd(x,0).
 \end{equation}
 2. 设$\{x_n\}$是可度量拓扑向量空间$X$的点列，如果$x_n\to 0(n\to \infty)$，则存在正标量$\gamma_n$满足$\gamma_n\to \infty$且$\gamma_nx_n\to 0$。

\begin{equation}
 \end{equation}

### 1.6 有界和连续

- **有界等价刻画**：设$E$是拓扑向量空间的子集，则如下两个命题等价：
 1. $E$有界；
 2. 对于$E$上的点列$\{x_n\}$和标量点列$\{\alpha_n\}$，如果$\alpha_n\to 0$($n\to\infty$)，则$\alpha_n x_n\to 0$($n\to \infty$)。
- **有界线性变换**：设$X$和$Y$是拓扑向量空间，映射$\Lambda:X\to Y$是线性的，如果$\Lambda$把有界集映射为有界集，即任意有界集$E\subset X$，$\Lambda(E)$是$Y$中的有界集，则称$\Lambda$是有界线性变换。
- **定理**：设$X$和$Y$是拓扑，映射$\Lambda:X\to Y$是线性的，则如下四个命题有关系$(a)\Rightarrow (b)\Rightarrow (c)$。如果$X$是可度量的，则四个命题等价即有$(c)\Rightarrow (d)\Rightarrow (a)$。     
 (a) $\Lambda$是连续的；   
 (b) $\Lambda$是有界的；   
 (c) 如果$x_n\to 0$，则$\{\Lambda x_n:n=1,2,3,\cdots\}$有界；   
 (d) 如果$x_n\to 0$，则$\Lambda x_n\to 0$。

\begin{equation}
 \end{equation}

### 1.7 半范数和局部凸性

- **半范数**：定义向量空间$X$上的实值函数$p$满足任意$x,y\in X$和标量$\alpha$有
 1. $p(x+y)\le p(x)+p(y)$,
 2. $p(\alpha x)=\vert \alpha \vert p(x)$,

 则称$p$是$X$的半范数。

 **可分的**：对于$X$上的半范数族$\mathcal{P}$，如果任意$x\neq 0$存在$p\in \mathcal{P}$满足$p(x)\neq 0$，则称$\mathcal{P}$是可分的。

- **吸收集**：对于拓扑向量空间$X$的凸集$E$，如果任意的$x\in X$，存在$t>0$满足$x\in t E$，则称$E$是吸收集。

 **Minkowski泛函**：集合$E$的Minkowski泛函是
 \begin{equation}
 \mu_{E}(x)=\inf \{t>0: x\in t E\}\  (x\in X).
 \end{equation}

- **定理**：设$p$是向量空间$X$的半范数则
 1. $p(0)=0$.
 2. $\vert p(x)-p(y)\vert \le p(x-y)$.
 3. $p(x)\ge 0$.
 4. $\{x:p(x)=0\}$是$X$的子空间。
 5. $B=\{x:p(x)<1\}$是均衡凸吸收集，且$p=\mu_{B}$.

- **定理**：设$A$是向量空间$X$上的凸吸收集，则
 1. $\mu_{A}(x+y)\le \mu_{A}(x)+\mu_{A}(y)$.
 2. 如果$t\ge 0$，则$\mu_{A}(tx)=t\mu_{A}(x)$.
 3. 如果$A$是均衡的，则$\mu_{A}$是半范数。
 4. 如果$B=\{x:\mu_{A}(x)<1\}$和$C=\{x:\mu_{A}(x)\le 1\}$，则$B\subset A\subset C$且$\mu_{A}=\mu_{B}=\mu_{C}$.

- **定理**：设$\mathcal{B}$是拓扑向量空间$X$的凸均衡局部基，任意$V\in \mathcal{B}$对应Minkowski泛函$\mu_{V}$，则
 1. 任意$V\in \mathcal{B}$，$V=\{x\in X:\mu_{V}(x)<1\}$.
 2. $\{\mu_{V}:V\in \mathcal{B}\}$是$X$上可分的连续半范数族。

- **定理**：假设$\mathcal{P}$是向量空间$X$上的可分半范族，任意$p\in \mathcal{P}$和$n\in\mathbb{Z}^{+ }$对应集合
 \begin{equation}
 V(p,n)=\{x:p(x)<\frac{1}{n}\}.
 \end{equation}
 设$\mathcal{B}$是由所有集合$V(p,n)$的有限交构成的集族。则$\mathcal{B}$是$X$的某个拓扑$\tau$构成的均衡凸局部基，在$\tau$下$X$是局部凸空间且
 1. 任意$p\in\mathcal{P}$是连续的。
 2. 集合$E\subset X$有界当且仅当所有$p\in\mathcal{P}$在$E$上有界。

- **定理**：
- **定理**：拓扑向量空间$X$是可赋范化的当且仅当在原点处有有界凸邻域。
\begin{equation}
 \end{equation}


### 1.8 商空间

- **商空间**：设$N$是向量空间$X$的子空间，对于任意$x\in X$，设$\pi(x)$是$N$的一个(包含$x$的)陪集：
 \begin{equation}
 \pi(x)=x+N.
 \end{equation}
 所有$N$的陪集构成线性空间称为$X$除以$N$的商空间$X/N$，对应的加法和数乘是
 \begin{equation}
 \pi(x)+\pi(y)=\pi(x+y),\ \ \alpha\pi(x)=\pi(\alpha x).
 \end{equation}
 **商映射**：$\pi$是$X$到$X/N$的线性映射，称为商映射，核为$N$。    
 **商拓扑**：设$\tau$是$X$上的向量拓扑，$N$是$X$的闭子空间。定义
 \begin{equation}
 \tau_{N}=\{E\subset X/N: \pi^{-1}(E)\in \tau\}.
 \end{equation}
 则$\tau_{N}$是$X/N$的拓扑，称为商拓扑。

- **定理**：设$N$是拓扑向量空间$X$的闭子空间，$\tau$是$X$的拓扑，$\tau_N$是如上定义的商拓扑。则
 1. $\tau_{N}$是$X/N$的向量拓扑，商映射$\pi:X\to X/N$是连续线性开映射。
 2. 如果$\mathcal{B}$是$\tau$的局部基，则集合族$\{\pi(V):V\in\mathcal{B}\}$是$\tau_{N}$的局部基。
 3. $X/N$继承了$X$的如下性质：局部凸、局部有界、可度量、可赋范。
 4. 如果$X$是F空间，或者Fréchet空间，或者Banach空间，则$X/N$也是。
- **应用**：设$N$和$F$是拓扑向量空间$X$的子空间，$N$是闭的，$F$是有限维的，则$N+F$是闭的。

- **半范数与商空间**：设$p$是向量空间$X$上的半范数且$N=\{x:p(x)=0\}$，$\pi$是$X$到$X/N$的商映射，定义
 \begin{equation}
 \tilde{p}(\pi(x))=p(x).
 \end{equation}
 则$\tilde{p}$是$X/N$的范数。


\begin{equation}
 \end{equation}


### 1.9 例子

- **$C(\Omega)$空间**：

- **$H(\Omega)$空间**：
- **$C^{\infty}$和$D_{k}$空间**：
- **$L^{p}$空间($0< p < 1$)**：

  

## 2 完备性

### 2.1 Baire纲

- **纲**：设$S$是一个拓扑向量空间，如果集合$E\subset S$满足闭包$\bar{E}$的内部是空集，则称$E$无处稠密。无处稠密集的可数并集称为$S$的第一纲集，如果$S$的子集不是第一纲集，则称为第二纲集。

- **Baire定理**：如果$S$是完备度量空间或者局部紧的Hausdorff空间，则$S$的任意一个可数稠密开集族的交集在$S$中也稠密。     
 **注**：之所以称为纲性定理，因为$S$是第二纲的。事实上，$\{E_i\}$是$S$的无处稠密的可数族，$V_i$是$\bar{E_i}$的补集，则$V_i$是稠密的，从Baire定理可知$\bigcap V_i\neq \varnothing$，所以$S\neq \bigcup E_i$，即$S$是第二纲的。    
 **证明**：

### 2.2 Banach-Steinhaus定理

- **等度连续**：设$X$和$Y$是两个拓扑向量空间，$\Gamma$是从$X$到$Y$的线性映射族，如果对于$Y$上$0$点的任意邻域$W$，存在$X$上$0$的邻域$V$满足：任意$\Lambda\in \Gamma$有，$\Lambda(V)\subset W$。则称$\Gamma$等度连续。

- **定理**：设$X$和$Y$是两个拓扑向量空间，$\Gamma$是从$X$到$Y$的等度连续线性映射族，则对于$X$的任意有界子集$E$，存在$Y$的有界子集$F$，使得任意$\Lambda\in \Gamma$有，$\Lambda(E)\subset F$。    
 **证明**：按定义易得，略。

- **一致有界原理(Banach-Steinhaus定理)**：设$X$和$Y$是两个拓扑向量空间，$\Gamma$是从$X$到$Y$的连续线性映射族，如果子集
 <div>
 \begin{equation}
 B=\{x\in X: \text{轨迹}\Gamma(x)=\{\Lambda x: \Lambda \in \Gamma,x\in B\}\text{在$Y$中有界}\}
 \end{equation}
</div>
 在$X$上是第二纲集，则$B=X$且$\Gamma$等度连续。    
 **证明**：由于$\Gamma(x)$有界，则任意的$0$的邻域$U$，存在$n\in \mathbb{Z}^{+}$使得
 \begin{equation}
 \Gamma(x)\subset n U,
 \end{equation}
 因此，$x\in n\bigcap_{\Lambda\in\Gamma}\Lambda^{-1}\bar{U}\overset{\bigtriangleup}{=}nE$。
 进而有
 \begin{equation}
 B\subset \bigcup_{n=1}^{\infty}nE,
 \end{equation}
 又因为$B$为第二纲集，故$\bigcup_{n=1}^{\infty}nE$为第二纲集，因此存在$n\in\mathbb{Z}^{+}$满足$nE$为第二纲集。再由于$x\to nx$是同胚映射，故$E$是第二纲集。而任意$\Lambda$连续，故$E$为闭集。因此存在$E$的内点$y$，故存在$0$的邻域$V\subset y-E$，有
 \begin{equation}
 \Lambda(V)\subset \Lambda(y)-\Lambda(E)\subset \bar{U}-\bar{U}.
 \end{equation}
 特别对于任意$Y$上$0$的邻域$W$，存在均衡邻域$U$，满足$\bar{U}+\bar{U}\subset W$，进而存在$V$满足对于任意$\Lambda\in\Gamma$
 \begin{equation}
 \Lambda (V)\subset \bar{U}+\bar{U}\subset W.
 \end{equation}
 即$\Gamma$是等度连续的。而由等度连续可得一致有界，特别任意$x\in X$，有$\Gamma(x)$有界，故$X=B$。

- **定理**：如果$\Gamma$是$F$空间$X$到拓扑向量空间$Y$的连续线性映射族，并且对于任意$x\in X$，集合
 \begin{equation}
 \Gamma(x)=\{\Lambda x:\Lambda \in \Gamma\}
 \end{equation}
 在$Y$中有界，则$\Gamma$是等度连续的。    
 **证明**

- **定理**：假设$X$和$Y$是拓扑向量空间，$\{\Lambda_n\}$是$X$到$Y$的连续线性映射序列。
 1. 如果子集
 \begin{equation}
 C=\{x\in X:\{\Lambda_n x\}\text{为$Y$中的Cauchy列}\}
 \end{equation}
 在$X$中是第二纲的，则$C=X$。
 2. 如果子集
 \begin{equation}
 L=\{x\in X: \Lambda x =\lim_{n\to \infty}\Lambda_n x\}
 \end{equation}
 是$X$中的第二纲集，$Y$是$F$空间，则$L=X$并且$\Lambda:X\to Y$是连续的。    
 **证明**

- **定理**：设$\{\Lambda_n\}$是从$F$空间$X$到拓扑向量空间$Y$中的连续线性映射序列，并且对于任意$x\in X$，有
 \begin{equation}
 \Lambda x=\lim_{n\to \infty}\Lambda_n x
 \end{equation}
 存在，则$\Lambda$是连续的。    
 **证明**

- **定理**：假设$X$和$Y$是拓扑向量空间，$K$是$X$中的凸紧集，$\Gamma$是$X$到$Y$中的连续线性映射族并且对于每个$x\in K$，轨道
 \begin{equation}
 \Gamma(x)=\{\Lambda x:\Lambda \in \Gamma\}
 \end{equation}
 在$Y$上有界，则存在有界集$B\subset Y$满足任意$\Lambda \in \Gamma$有$\Lambda(K)\subset B$.    
 **证明**




\begin{equation}
 \end{equation}


### 2.3 开映射定理

- **开映射**：设映射$f$从拓扑空间$S$到拓扑空间$T$。对于点$p\in S$，如果$p$的任意邻域$V$存在$f(p)$的一个邻域包含于$f(V)$，则称$f$在$p$点是开的。如果$S$上的任意开集$U$有$f(U)$是$T$上的开集，则称$f$是$S$上的开映射。

- **开映射定理**：设$X$是$F$空间，$Y$是拓扑向量空间，$\Lambda:X\to Y$是连续线性映射，且$\Lambda(X)$是$Y$中的第二纲集。则
 1. $\Lambda(X)=Y$;
 2. $\Lambda$是一个开映射；
 3. $Y$是$F$空间。     
 **证明**：

- **推论**：
 1. 如果$\Lambda$是从$F$空间$X$到$F$空间$Y$的连续线性满射，则$\Lambda$是开的。
 2. 如果上一条的$\Lambda$还满足一一映射，在$\Lambda^{-1}:Y\to X$是连续的。
 3. 设$X$和$Y$是Banach空间，如果$\Lambda:X\to Y$是连续线性双射，则存在实数$a,b>0$满足任意的$x\in X$有
 \begin{equation}
 a\Vert x\Vert \le \Vert \Lambda x\Vert \le b\Vert x\Vert.
 \end{equation}
 4. 设$\tau_1\subset \tau_2$是线性空间$X$上的线性拓扑，如果$(X,\tau_1)$和$(X,\tau_2)$是$F$空间，则$\tau_1=\tau_2$.

\begin{equation}
 \end{equation}

### 2.4 闭图像定理

- **图像**：设$f$是集合$X$到$Y$的映射，则Cartesian积$X\times Y$的子集
 \begin{equation}
 \{(x,f(x)):x\in X\}
 \end{equation}
 称为$f$的图像。
- **命题**：如果$X$是拓扑空间，$Y$是Hausdorff空间，且$f:X\to Y$连续，则$f$的图像是闭的。

- **闭图像定理**：设$X$和$Y$是F空间，$\Lambda:X\to Y$是线性的，$G=\{(x,\Lambda x): x\in X\}$在$X\times Y$上是闭的，则$\Lambda$连续。


### 2.5 双线性映射

- **双线性映射**：设$X,Y,Z$是向量空间，$B$是$X\times Y$到$Z$的映射。对于任意的$x\in X$或$y\in Y$，定义映射
 \begin{equation}
 B_x(y)=B(x,y)=B^{y}(x),
 \end{equation}
 如果所有$B_x(y)$和$B^{y}(x)$都是线性映射，则称$B$是双线性的。

- **分别连续**：如果$X,Y,Z$是拓扑向量空间，并且所有$B_x$和$B^y$是连续的，则称$B$是分别连续的。

- **定理**：假设$B:X\times Y\to Z$是双线性并且分别连续，$X$是F空间，$Y$和$Z$是拓扑向量空间。则任意$X$中$x_n\to x_0$和$Y$中$y_n\to y_0$有$Z$中
 \begin{equation}
 B(x_n,y_n)\to B(x_0,y_0).
 \end{equation}
 如果$Y$可度量化，则$B$连续。

### 2.6 习题




## 3 凸性

### 3.1 Hahn-Banach 定理

- **对偶空间**：拓扑向量空间$X$的对偶空间$X^{* }$是$X$上的所有连续线性泛函组成的空间。其中加法和数乘的定义为
 \begin{equation}
 (\Lambda_1+\Lambda_2)x=\Lambda_1 x+\Lambda_2 x,\ \ (\alpha \Lambda)x=\alpha\cdot \Lambda x.
 \end{equation}

- **控制延拓定理1**：假设$M$是实向量空间$X$的子空间，$p:X\to R$
 满足任意的$x,y\in X$和$t\ge 0$有
 \begin{equation}
 p(x+y)\le p(x)+p(y),\ \ p(tx)=tp(x),
 \end{equation}
 $f:M\to R$是线性的且在$M$上有$f(x)\le p(x)$。则存在线性映射$\Lambda:X\to R$满足
 \begin{equation}
 \Lambda x=f(x)\ \ (x\in M),
 \end{equation}
 且
 \begin{equation}
 -p(-x)\le \Lambda x\le p(x), (x\in X).
 \end{equation}

- **控制延拓定理2**：设$M$是向量空间$X$的子空间，$p$是$X$的半范数，且$f$是$M$上的线性泛函满足
 \begin{equation}
 \vert f(x)\vert \le p(x)\ \ (x\in M).
 \end{equation}
 则$f$可延拓为$X$上的线性泛函$\Lambda$且满足
 \begin{equation}
 \vert \Lambda x\vert \le p(x)\ \ (x\in X).
 \end{equation}
 **推论**：如果$X$是赋范空间且$x_0\in X$，则存在$\Lambda \in X^* $满足任意$x\in X$有
 \begin{equation}
 \Lambda x_0=\Vert x_0\Vert,\ \ \vert \Lambda x\vert \le \Vert x\Vert.
 \end{equation}


- **分离定理**：假设$A$和$B$是拓扑向量空间$X$上的互不相交的非空凸集，
 1. 如果$A$是开集则存在$\Lambda \in X^{* }$和$\gamma\in \mathbb{R}$满足对于任意$x\in A$和$y\in B$有
 \begin{equation}
 Re \Lambda x< \gamma <Re \Lambda y.
 \end{equation}
 2. 如果$A$是紧集，$B$是闭集，$X$局部凸，则存在$\Lambda \in X^{* }$,$\gamma_1,\gamma_2\in\mathbb{R}$满足任意$x\in A$和$y\in B$有
 \begin{equation}
 Re \Lambda x< \gamma_1 <\gamma_2 <Re \Lambda y.
 \end{equation}
 **推论**：如果$X$是局部凸开集，则$X^ * $在$X$上有分离性。    
 **定理**：设$M$是局部凸开集$X$的子空间，且$x_0\in X$。如果$x_0$不属于$M$的闭包，则存在$\Lambda \in X^{* }$满足$\Lambda x_0=1$，但是任意$x\in M$有$\Lambda x=0$。    
 **定理**：设$B$是局部凸空间$X$上的均衡闭凸集，$x_0\in X$但$x_0 \notin B$。则存在$\Lambda\in X^{* }$满足任意$x\in B$，$\vert x\vert \le 1$，但$\Lambda x_0 > 1$。

- **连续延拓定理**：设$M$是局部凸空间$X$的子空间，如果$f$是$M$上的连续映射，则存在$\Lambda\in X^{* }$满足在$M$上$\Lambda=f$。

### 3.2 弱拓扑

- **拓扑的强弱**：设$\tau_1$和$\tau_2$是集合$X$上两个拓扑，如果$\tau_1\subset \tau_2$，则$\tau_1$的开集也是$\tau_2$的开集，故称$\tau_1$比$\tau_2$弱或者$\tau_2$比$\tau_1$强。     
 **注1**：上面的包含关系不排除等号。    
 **注2**：恒等映射是$(X,\tau_2)$到$(X,\tau_1)$的连续映射，是$(X,\tau_1)$到$(X,\tau_2)$的开映射。
- **弱拓扑**：设$X$是集合，$\mathcal{F}$是由映射$f:X\to Y_{f}$($Y_{f}$是拓扑空间)组成的非空映射族。使得任意$f\in \mathcal{F}$都连续的最弱拓扑称为$X$由$\mathcal{F}$诱导的弱拓扑，也称为$X$的$\mathcal{F}$-拓扑。其实是集合
 \begin{equation}
 \{f^{-1}(V) : f \in \mathcal{F}, V\text{是}Y_{f}\text{中的开集}\}
 \end{equation}
 通过有限交和无限并生成的集合。

- **引理**：设$\Lambda_1,\Lambda_2,\cdots,\Lambda_n$和$\Lambda$是向量空间$X$上的线性泛函。设
 \begin{equation}
 N=\{x:\Lambda_1 x=\cdots =\Lambda_n x=0\},
 \end{equation}
 则如下三个性质等价：
 1. 存在标量$\alpha_1,\cdots,\alpha_n$满足
  \begin{equation}
  \Lambda = \alpha_1 \Lambda+\cdots +\alpha_n\Lambda_n.
  \end{equation}
 2. 存在$\gamma<\infty$满足
  \begin{equation}
  \vert \Lambda \vert\le \gamma\max_{1\le i\le n}\vert \Lambda_{i}x\vert,\ \ (x\in X).
  \end{equation}
 3. 对于任意$x\in N$，有$\Lambda x=0$。
- **定理**：设$X$是向量空间，$X'$是$X$上的线性泛函组成的可分向量空间，则$X$在$X'$-拓扑构成局部凸空间，且对偶是$X'$。
- **拓扑向量空间的弱拓扑**：设$X$是拓扑向量空间，它的对偶空间$X^{* }$在$X$上可分，则$X$的$X^{* }$-拓扑称为$X$的弱拓扑。
- **定理**：设$E$是局部凸空间$X$的凸子集，则$E$的弱闭包等于闭包。     
 **推论**：对于局部凸空间的闭子集，闭等价于弱闭，稠密等价于弱稠密。
- **定理**：设$X$是可度量的局部凸空间，如果$X$中的序列$\{x_n\}$弱收敛于某个$x\in X$，则存在$X$中的序列$y_{n}$满足
 1. 每个$y_i$是有限个$x_n$的凸组合。
 2. $y_i$收敛于$x$。
- **弱$* $拓扑**：设$X$是拓扑向量空间，对偶空间为$X^{* }$，则$X^{* }$的$X$拓扑称为$X^{* }$的弱$* $拓扑。

### 3.3 紧凸集

- **Banach-Alaoglu定理**：设$V$是拓扑向量空间$X$中$0$的邻域，如果
 \begin{equation}
 K=\{\Lambda \in X^{* }:\vert \Lambda \vert\le 1, x\in V\},
 \end{equation}
 则$K$是弱$* $紧的。
- **定理**：设$X$是可分拓扑向量空间，如果$K\subset X^{* }$，且$K$是弱$* $紧的，则$K$在弱$* $拓扑下可度量化。
- **定理**：设$V$是可分拓扑向量空间$X$中$0$的邻域，如果$X^{* }$中的序列$\{\Lambda_n\}$满足
 \begin{equation}
 \vert \Lambda_n x\vert \le 1,\ \ (x\in X,\ n=1,2,\cdots)
 \end{equation}
 则存在子列$\{\Lambda_{n_i}\}$和$\Lambda \in X^{* }$使得
 \begin{equation}
 \lim_{i\to \infty}\Lambda_{n_i}x=\Lambda x,\ \ (x\in X)
 \end{equation}
- **定理**：局部凸空间$X$中，弱有界等价于有界。
- **推论**：如果$X$是赋范空间，$E\subset X$且
 \begin{equation}
 \sup_{x\in E}\vert \Lambda x\vert < \infty \ \ (\Lambda \in X^{* }).
 \end{equation}
 则存在$\gamma<\infty$满足
 \begin{equation}
 \Vert x\Vert < \gamma \ \ (x\in E).
 \end{equation}
- **定义**：(a)设$X$是向量空间且$E\subset X$，定义$E$的凸包是$X$中所有包含$E$的凸子集的交集，记作$co(E)$。等价的有
 \begin{equation}
 co(E) = \{ \sum_{j=1}^n t_j x_j\, : x_j \in E,\, \sum_{j=1}^n t_j = 1,\, t_j \in \lbrack 0, 1 \rbrack \, \}
 \end{equation}
 (b)设$X$是向量空间且$E\subset X$，定义$E$的闭凸包是$co(E)$的闭包，记作$\overline{co}(E)$。    
 (c)设$X$是距离空间且$E\subset X$，如果任意$\varepsilon >0$，$E$包含于有限个半径为$\varepsilon$的开球的并集中，则称$E$完全有界。   
 (d)设$X$是拓扑向量空间且$E\subset X$，如果$X$中任意$0$的邻域$V$，存在有限集$F$满足$E\subset F+V$，则称$E$完全有界。
- **定理**：(a)如果$A_1,A_2,\cdots,A_n$是拓扑向量空间$X$中的凸紧集，则$co(A_1\bigcup\cdots \bigcup A_n)$是紧的。    
 (b)设$X$是局部凸拓扑向量空间且$E\subset X$完全有界，则$\overline {co}(E)$是紧的。   
 (c)设$X$是Fréchet空间且$K\subset X$是紧的，则$\overline{co}(K)$是紧的。   
 (d)如果$K$是$\mathbb{R}^{n}$中的紧集，则$\overline{co}(K)$是紧的。   
- **命题**：如果$E\subset \mathbb{R}^{n}$，$x\in co(E)$，则$x$属于$E$的某个最多包含$n+1$个元素的子集中。
- **定理**：设$X$是拓扑向量空间，$X^{* }$在$X$上可分，如果$A$和$B$是$X$种互不相交的非空紧凸集，则存在$\Lambda \in X^{* }$使得
 \begin{equation}
 \sup_{x\in A}\Re{\Lambda x}< \inf_{x\in B}\Re{\Lambda x}.
 \end{equation}
- **端点**：设$K$是向量空间$X$的子集，且$S\subset K$，如果$x,y\in S$，$0< t< 1$且
 \begin{equation}
 tx+(1-t)x\in S,
 \end{equation}
 则$x,y\in S$。我们就称$S$是$K$的端子集。一个点构成的端子集称为端点。所有的端点记作$E(K)$。
- **Krein-Milman定理**：设$X$是拓扑向量空间，$X^{* }$在$X$上可分，如果$K$是$X$的非空紧凸集，则$K$是它的端点集合的闭凸包，即$K=co(E(K))$。
- **定理**：如果$K$是局部凸空间的紧子集，则$K\subset \overline{co}(E(K))$。
- **Milman定理**：如果$K$是局部凸空间的紧集且$\overline{co}(K)$也是紧的，则$\overline{co}(K)$的每一个端点属于$K$。


<!-- ### 3.4 向量值积分

- **定义**：
- **定理**：
- **定理**：

### 3.5 全纯函数

- **定义**：
- **定理**：
- **定理**： -->

<!-- ### 3.6 习题 -->



## 4 Banach空间的对偶

### 4.1 赋范空间的赋范对偶

- **$\mathcal{B}(X,Y)$**：$\mathcal{B}(X,Y)$表示所有$X$到$Y$的有界线性映射。

- **$\mathcal{B}(X,Y)$是赋范线性空间**：设$X$和$Y$是赋范线性空间，定义$\mathcal{B}(X,Y)$上的函数
 \begin{equation}
 \Vert \Lambda \Vert =\sup\{\Vert \Lambda x\Vert:x\in X,\Vert x\Vert \le 1\}
 \end{equation}
 则$\mathcal{B}(X,Y)$是赋范线性空间，且如果$Y$是Banach空间，则$\mathcal{B}(X,Y)$是Banach空间。

- **定理**：设$B$是赋范空间$X$上的闭单位球，对于任意$x^{* }\in X^{* }$定义
 \begin{equation}
 \Vert x^{* }\Vert =\sup{\{\vert \langle x,x* \rangle \vert : x\in B\}}.
 \end{equation}
 则有
 1. $X^{* }$在所定义范数是Banach空间。
 2. 设$B^{* }$是$X^{* }$上的闭单位球，对于任意$x\in X$，有
  \begin{equation}
  \Vert x\Vert =\sup{\{\vert \langle x,x^{* }\rangle\vert:x^{* }\in B^{* }\}}.
  \end{equation}
  故$x^{* }\to\langle x,x^{* }\rangle $是$X^{* }$上的有界线性泛函，并且范数是$\Vert x\Vert$。
  3. $B^{* }$是弱$* $紧的。
- **有界线性算子范数等价刻画**：设$X,Y$是赋范空间，如果$\Lambda \in \mathcal{B}(X,Y)$，则
 \begin{equation}
 \Vert \Lambda \Vert =\sup{\{\langle\Lambda x,y\rangle:\Vert x\Vert \le 1,\Vert y^{* }\Vert \le 1\}}.
 \end{equation}

- **自反空间**：设$X$是赋范空间，如果$X=X''$，则称$X$是自反的，其中等号是等距同构的意义，另外一般的赋范空间只满足$X\subset X''$。
- **零化子**：设$X$是Banach空间，$M$是$X$的子空间，$N$是$X^{* }$的子空间(并没有假设$M$和$N$是闭的)，定义他们的零化子
 \begin{equation}
 M^{\bot}=\{x^{* }\in X^{* }:\forall{x\in M},\langle x,x^{* }\rangle=0\}
 \end{equation}
 \begin{equation}
 ^{\bot}{N}=\{x\in X:\forall{x^{* }\in N},\langle x,x^{* }\rangle=0\}
 \end{equation}
- **零化子性质**：在零化子的假设下，有
 1. $^{\bot}(M^{\bot})$是$M$在$X$的闭包。
 2. $(^{\bot}N^{})^{\bot}$是$N$在$X^{* }$的弱$* $ 闭包。

- **定理**：设$M$是Banach空间$X$的闭子空间，
 1. 任意$m^{* }\in M^{* }$可通过Hahn-Banach定理延拓到$x^{* }\in X^{* }$，定义映射
  \begin{equation}
  \sigma x^{* }=x^{* }+M^{\bot},
  \end{equation}
  则$\sigma$是$M^{* }$到$X^{* }/M^{\bot}$的等距同构。
 2. 设$\pi:X\to X/M$的商映射，记$Y=X/M$，对于任意$y^{* }\in Y^{* }$，定义
  \begin{equation}
  \tau y^{* }=y^{* }\pi,
  \end{equation}
  则$\tau$是$Y^{* }$到$M^{\bot}$上的等距同构。


### 4.2 伴随算子

- **定理**：设$X$和$Y$是赋范空间，对于任意的$T\in \mathcal{B}(X,Y)$，存在唯一的$T^{* }\in \mathcal{B}(Y^{* },X^{* })$满足对任意$x\in X$，$y^{* }\in Y^{* }$有
 \begin{equation}
 \langle Tx,y^{* }\rangle = \langle x,T^{* }y^{* }\rangle.
 \end{equation}
 且有
 \begin{equation}
 \Vert T^{* }\Vert =\Vert T\Vert.
 \end{equation}
- **核空间和值域**：对于$X$到$Y$的映射$T$，$T$的核空间$\mathcal{N}(T)$和值域$\mathcal{R}(T)$是
 \begin{equation}
 \mathcal{N}(T)=\{x\in X: Tx=0\}
 \end{equation}
 \begin{equation}
 \mathcal{R}(T)=\{Tx\in Y:x\in X\}.
 \end{equation}

- **定理**：设$X$和$Y$是Banach空间，$T\in\mathcal{B}(X,Y)$，则
 \begin{equation}
 \mathcal{N}(T^{* })=\mathcal{R}(T)^{\bot},\ \ \mathcal{N}(T)=^{\bot}\mathcal{R}(T^{* }).
 \end{equation}
 **推论**：
 1. $\mathcal{N}(T^{* })$在$Y^{* }$中弱$* $闭。
 2. $\mathcal{R}(T)$在$T$中稠密等价于$T^{* }$是单射。
 3. $T$是单射等价于$\mathcal{R}(T^{* })$在$X^{* }$中弱$* $稠密。

- **定理**：设$U$和$V$分别是Banach空间$X$和$Y$的开单位球，如果$T\in \mathcal{B}(X,Y)$且$\delta >0$，则有(a)$\to$(b)$\to$(c)$\to$(d)成立.其中    
 (a) 任意$y^{* }\in Y^{* }$，有$\Vert T^{* }y^{* }\Vert \ge \delta \Vert y^{* } \Vert$.    
 (b) $\delta V \subset \overline{T(U)} $.    
 (c) $\delta V \subset T(U) $.    
 (d) $T(X)=Y$.   
 如果只有(d)成立，则存在$\delta >0$使得(a)成立。

- **定理**：设$X$和$Y$是Banach空间，$T\in \mathcal{B}(X,Y)$，则以下三个命题等价
 1. $R(T)$在$Y$中是闭的。
 2. $R(T^{* })$在$X^{* }$中是弱$* $闭的。
 3. $R(T^{* })$在$X^{* }$中是以范数闭的。    
 **注**：$R(T)$在$Y$中是闭的等价于$R(T)$是弱$* $闭的，但是在$X^{* }$中以范数闭的不一定是弱$* $闭的。

- **定理**：设$X$和$Y$是Banach空间，$T\in \mathcal{B}(X,Y)$，则$\mathcal{R}(T)=Y$当且仅当$T^{* }$是单射且$\mathcal{R}(T^{* })$是以范数闭的。

### 4.3 紧算子

- **紧算子**：设$X$和$Y$是Banach空间，$U$是$X$的单位球，对于线性映射$T: X\to Y$，如果$T(U)$的闭包在$Y$中是紧的，则称$T$是紧算子。    
 **注**：
 1. 显然$T$有界，故$T\in \mathcal{B}(X,Y)$。
 2. 由于$Y$是完备度量空间，故$Y$中具有紧闭包的子集等价于完全有界集，因此$T$是紧集等价于$T(U)$是完全有界集。
 3. $T$是紧的等价于对于$X$中的任意有界序列$\{x_n\}$，存在子列$\{x_{n_{i}}\}$在$Y$中收敛。

- **定义**
 1. 设$X$是一个Banach空间，则$\mathcal{B}(X)$不仅是Banach空间，而且是一个代数，即如果$T,S\in \mathcal{B}(X)$，定义$ST\in \mathcal{B}(X)$：
 \begin{equation}
 ST(x)=S(T(x)),\ \ (x\in X).
 \end{equation} 
 显然有不等式
 \begin{equation}
 \Vert ST \Vert =\Vert S\Vert \Vert T\Vert.
 \end{equation} 
 特别可以定义$ST\in \mathcal{B}(X)$的幂，$T^{0}=I$，$T^{n}=TT^{n-1}$，$n=2,3,\cdots$。
 2. 对于算子$T\in \mathcal{B}(X)$，如果存在$S\in \mathcal{B}(X)$满足
 \begin{equation}
 ST=I=TS,
 \end{equation}
 则称$T$为可逆的，记$S=T^{-1}$。通过开映射定理，$T$可逆当且仅当$\mathcal{N}(T)=\{0\}$且$\mathcal{R}(T)=X$。
 3. 算子$T\in \mathcal{B}(X)$的谱$\sigma (T)$是使得$T-\lambda I$不可逆的所有$\lambda$组成的集合。因此$\lambda \in \sigma(T)$等价于$T-\lambda I$非双射。如果$\lambda \in \sigma(T)$不是单射，则称$\lambda$是特征值，对应特征空间是$\mathcal{N}(T-\lambda I)$，任意$x\in \mathcal{N}(T-\lambda I)(x\neq 0)$是$T$的特征向量。

- **定理**：设$X$和$Y$是Banach空间，
 1. 如果$T\in \mathcal{B}(X,Y)$且$\dim(\mathcal{R}(T))<\infty$，则$T$是紧的。
 2. 如果$T\in \mathcal{B}(X,Y)$是紧的，且$\mathcal{R}(T)$是闭的，则$\dim(\mathcal{R}(T))<\infty$。
 3. 紧算子以它的范数拓扑构成$\mathcal{B}(X,Y)$的一个闭子空间。
 4. 如果$T\in \mathcal{B}(X)$是紧的，且$\lambda\neq 0$，则$\dim(\mathcal{R}(T-\lambda I))<\infty$.
 5. 如果$\dim{X}=\infty$，$T\in \mathcal{B}(X)$是紧的，则$0\in \sigma(T)$.
 6. 如果$S,T\in \mathcal{B}(X)$且$T$是紧的，则$ST$和$TS$也是紧的。
- **定理**：设$X$和$Y$是Banach空间，且$T\in\mathcal{B}(X,Y)$，则$T$是紧的当且仅当$T^{* }$是紧的。

- **直和**：设$M$是拓扑向量空间$X$的闭子空间，如果存在$X$的闭子空间$N$满足
 \begin{equation}
 X=M+N,\ \ M\bigcap N=\{0\},
 \end{equation}
 则称$M$在$X$中可余，$X$为$M$和$N$的直和，记作
 \begin{equation}
 X=M\oplus N.
 \end{equation}

- **引理**：设$M$是拓扑向量空间的闭子空间，
 1. 如果$X$局部凸且$\dim{M}<\infty$，则$M$在$X$可余。
 2. 如果$\dim{X/M}<\infty$，则$M$在$X$可余。$\dim{X/M}<\infty$也叫做$M$在$X$的余维数。
- **引理**：设$M$是赋范空间的子空间，如果$M$在$X$不稠密，且$r>1$，则存在$x\in X$满足
 \begin{equation}
 \Vert x\Vert < r,\ \ \Vert x-y\Vert \ge 1(y\in M).
 \end{equation}
- **定理**：如果$X$是Banach空间，$T\in \mathcal{B}(X)$是紧的,且$\lambda \neq 0$，则$T-\lambda I$的值域是闭的。
- **定理**：设$X$是Banach空间，$T\in \mathcal{B}(X)$是紧的，$r>0$，$T$的所有特征值$\lambda$中满足$\vert \lambda \vert >r$的部分组成的集合$E$，则任意$\lambda \in E$，$\mathcal{R}(T-\lambda I)\neq X$且$E$是有限集。
- **定理**：设$X$是Banach空间，$T\in\mathcal{B}(X)$是紧的，则
 1. 如果$\lambda$则
  \begin{equation}
  \dim{\mathcal{N}(T-\lambda I)}=\dim{\mathcal{N}(T^{* }-\lambda I)} = \dim{X/\mathcal{R}(T-\lambda I)} = \dim{X^{* }/\mathcal{R}(T^{* }-\lambda I)}
  \end{equation}
  为有限值。
 2. 如果$\lambda\neq 0$且$\lambda \in \sigma(T)$，则$\lambda$是$T$和$T^{* }$的特征值。
 3. $\sigma(T)$是至多可数个元素的紧集，且至多有一个极限点$0$。

<!-- ### 习题 -->



<!-- ## 5 一些应用

### 5.1 一个连续定理

### 5.2 $L^{p}$空间的闭子空间

### 5.3 向量值测度的范围

### 5.4 一般的Stone-Weierstrass 定理

### 5.5 两个插值定理

### 5.6 Kakutani不动点定理

### 5.7 紧群上的Haar测度

### 5.8 不可余子空间

### 5.9 Poisson核的和

### 5.10 另两个不动点定理

### 习题 -->


