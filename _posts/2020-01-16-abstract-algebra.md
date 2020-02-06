---
layout: post
title:  "抽象代数基础"
date:   2020-01-16 03:54:49 +0800
categories: math
tags: algebra
---

# 抽象代数基础


## 一. 基本概念

### 1. 集合和映射

*目标：*
理解集合与映射的概念，掌握集合之间的运算，能够在集合之间建立映射关系，并判断两个映射是否相同。

*内容：*
- **集合**（英语：Set，或简称集）是基本的数学概念，它是集合论的研究对象，指具有某种特定性质的事物的总体，（在最原始的集合论─朴素集合论─中的定义，集合就是“一堆东西”。）集合里的事物（“东西”），叫作元素。若然$x$是集合$A$的元素，记作$x\in A$。

- **集合运算** 交并差

### 2. 代数运算

*目标：*
掌握代数运算与映射的关系，能够建立有限集合之间的运算表，并判断给定的运算是否满足结合律、交换律以及两种分配律。

*内容：*

### 3. 同态映射、同构映射和自同构

*目标：*掌握同态映射、同构映射和自同构的概念，理解同态与同态满射（满同态）的关系，并能判定映射是否是同态满射（满同态），掌握具有同态满射（满同态）的集合之间的联系。能够判定给定的映射和运算是否是同构关系，能建立两个集合之间的同构映射。

*内容：*

### 4. 关系和等价关系

*目标：*
理解关系和等价关系的概念，掌握等价关系和分类之间的转换定理，熟练判定给定的关系是否是等价关系。并熟悉剩余类的基本特性，能够建立整数间给定模的剩余类

*内容：*

## 二. 群

### 1. 群的定义

*目标：*
掌握群的等价定义和例子，理解左、右单位元，左、右逆元的意义，掌握有限群、无限群、群的阶和交换群的概念。充分掌握单位元、逆元的存在性和唯一性，了解消去律的定义，能熟练掌握群与阶的关系，会计算群元素的阶。

*内容：*
- **半群**： 在非空集合$G$上有运算"$\circ$"，且满足结合律即：任意的$a,b,c \in G$， 有$(a\circ b) \circ c = a\circ (b\circ c)$，则称$\{G, \circ \}$是一个半群。

- **群**：对于非空集合$G$，在$G$上定义运算"$\circ$"满足：  
(1)运算封闭：任意的$a,b\in G$，有$a\circ b \in G$;  
(2)结合律：任意的$a,b,c \in G$， 有$(a\circ b) \circ c = a\circ (b\circ c)$;  
(3)存在单位元：存在$e\in G$，满足任意的$a\in G$，有$a \circ e= e\circ a =a$;  
(4)存在逆元：任意$a\in G$，存在$b\in G$满足$a\circ b = b\circ a = e$;  
则称$\{G, \circ \}$是一个群。

- **交换群**：如果群$G$满足交换律，即：任意的$a,b \in G$，有$a\circ b =b \circ a$，称群$G$为交换群，或者Abel群。

- **有限群**：群$G$的元素个数有限。
- **无限群**：群$G$的元素个数无限。
- **群的阶**：群$G$的元素个数$ \| G \| $。

- **消去律**：设$G$为群，任意$a,b,c\in G$，如果$ab=ac$， 则$b=c$.
- **元素的阶**：设$G$为群，对于$a\in G$，如果任意的$k\in \mathbb{N}$，有$a^k \neq e$，则称$a$的阶为无穷，如果存在$k\in \mathbb{N}$，满足$a^k = e$，则称$\min \{ k\in \mathbb{N} :a^k=e\}$为$a$的阶。
- **群与阶的关系**：设$a$为群$G$的一个元素，则  
(1)$a$的阶为无穷 $\Leftrightarrow$ 任意$m,n\in G, m\neq n$,有$a^m\neq a^n$;  
(2)$a$的阶为$d$，则i)$h\in \{h\in \mathbb{Z}:a^h=e\}$ $\Leftrightarrow$ $d|h$, ii)$(m,n)\in\{(m,n):m,n\in \mathbb{Z}, a^m=a^n\}$ $\Leftrightarrow$ $d|(m-n)$ $\Leftrightarrow$ $m\equiv n \pmod{d}$;  
(3)$a$的阶为$d$，$k\in \mathbb{N}$，则i)$a^k$的阶为$d/(d,k)$，$(d,k)$为$d,k$的最大公因数，
ii)$a^k$的阶为$d$ $\Leftrightarrow$ $(d,k)=1$;  
(4)$b\in G$，$a$的阶为$m$，$b$的阶为$n$，$ab=ba$，$(m,n)=1$，则$ab$阶为$mn$.

### 2. 同构和同态

*目标：*
理解群同构、同态的定义，掌握一个群的自同构的集合也成群的证明，掌握群同态的有关性质，并能证明在同态下，单位元的像也是单位元，元 $a$ 的逆元的像是 $a$ 的像的逆元。

*内容：*

- **同态**：设$G,G'$为两个群，如果有$G$到$G'$的映射$\sigma$满足：任意$a,b\in G$，有
$$\sigma (ab) = \sigma (a) \sigma (b),$$
则称$\sigma$为$G$到$G'$的一个同态映射，简称同态(homomorphism).
- **同构**：设$G,G'$为两个群，如果有$G$到$G'$的双射(既是单射又是满射)$\sigma$满足：任意$a,b\in G$，有
$$\sigma (ab) = \sigma (a) \sigma (b),$$
则称$\sigma$为$G$到$G'$的一个同构映射，简称同构(isomorphism)，$G$和$G'$同构记作$G\cong G'$.
- **自同构**：群$G$到自身的一个同构映射成为$G$的自同构。(所有自同构映射组成的集合，对于映射乘法构成群。)
- **群同态的性质**：设$\sigma$是群$G$到群$G'$的一个同态，则  
(1)$\sigma$把$G$的单位元$e$映射成$G'$的单位元$e'$;  
(2)$\sigma(a^{-1})=\sigma(a)^{-1}$，任意$a\in G$;  
(3)$G$的子群$H$在$\sigma$下的像$\sigma(H)$是$G'$的子群；  
(4)$G$在$\sigma$下的像$Im\sigma$是$G'$的子群，称$Im\sigma$是同态$\sigma$的像。


### 3. 循环群和剩余类加群

*目标：*
掌握循环群的定义和由生成元决定循环群的性质与特点，熟练掌握剩余类加群，并能证明任一循环群可以与整数加群或模为$n$的剩余类加群同构。以及与循环群同态的群的性质。

*内容：*
- **循环群**：如果群$G$的每一个元素都能写成$G$中某一个元素$a$的幂次，则称$G$为循环群，把$a$叫做$G$的生成元，可以记作$\langle a \rangle$.
- **等价条件**：群$G$是循环群等价于$G$由一个元素生成。
- **剩余类群**：模$m$剩余类环$\mathbb{Z}_ {m}$关于加法构成一个循环群，所有可逆元素组成的集合关于乘法构成Abel群，称为$\mathbb{Z}_ {m}$的单位群，记作 $\mathbb{Z}^{* }_ {m}$.
- **循环群与Abel群**：设$G$为有限Abel群，则$G$中存在一个元素，它的阶是每个元素的倍数。  
设$G$为有限Abel群则$G$为有限群当且仅当对于任意正整数$m$，方程$x^m=e$在$G$中的根不超过$m$个。
- **循环群的同构**：任意无限循环群都与$\mathbb{Z}$同构，任意$m$阶循环群都与 $\mathbb{Z}_ {m}$ 同构。


### 4. 变换群

*目标：*
熟练掌握变换的符号的运用和变换的乘法，能证明可以成群的变换只包含一一变换，且单位元一定是恒等变换。了解变换群的定义和性质。掌握任何一个群都同一个变换群同构的定理的证明。掌握元素求逆等运算。

*内容：*


### 5. 置换群

*目标：*
理解置换与置换群的定义与性质，掌握每一个 n 元置换都可以写成若干个互相没有共同数字（不相连）的循环置换（轮换）的乘积的证明与运用。理解有限群与置换群的同构关系。

*内容：*
- **全变换群**：非空集合$\Omega$到自身的所有双射组成的集合，对于映射的乘法成一个群，称其为集合$\Omega$的全变换群，记作$S_{\Omega}$.
- **置换**：对于有限集合$\Omega$，$\Omega$到自身的一个双射叫做$\Omega$的一个置换。当$\Omega$含有$n$铬元素时，置换被称为$n$元置换，$\Omega$的全变换群被称为$n$元对称群，记作$S_n$.
- **置换群**：$n$元对称群$S_n$的任一子群称为$n$元置换群。
- **变换群**：非空集合$\Omega$的全变换群的任一子群称为$\Omega$的变换群。

### 6. 子群

*目标：*
掌握子群的定义，掌握群的子集成群的充分必要的条件与判定定理，并能掌握找出已知群的子群的一般方法，了解群与子群中的单位元与逆元的关系，以及子群与子群之间的关系。

*内容：*
- **子群**：群$G$的非空子集$H$如果对于$G$的运算也成一个群，则称$H$是$G$的子群(subgroup).
- **等价条件**：设$H$是群$G$的非空子集，则$H$是$G$的子群等价于任意$a,b\in H$, 有$ab^{-1}\in H$.
- **由$S$生成的子群**：设$S$为群$G$的非空子集，则所有包含$S$的子群的交仍是群，称为由$S$生成的子群，记作$\langle S \rangle$. 其实，
$$\langle S \rangle=\{ x_1^{m_1}x_2^{m_2}\cdots x_k^{m_k} | x_i\in S, m_i\in \mathbb{Z}, 1\le i \le k, k\in \mathbb{Z}^{+}\}.$$

### 7. 陪群

*目标：*
掌握陪集的定义，以及与等价关系和分类之间的关系，了解子群与陪集之间的关系，并能证明有限群的阶能被元的阶整除的定理，以及阶为素数的群一定为循环群的证明。

*内容：*
- **左陪集**：设$H$为群$G$的子群，$a$为$G$中元素，定义$aH=\{ah \| h\in H\}$，称$aH$为子群$H$的左陪集。
- **左陪集与等价关系**：同一左陪集中的两个元素，可以定义为等价。
- **左陪集与分类**：子群$H$的所有左陪集组成的集合是$G$的一个分类。
- 子群$H$的任意两个左陪集要么相等要么不相交。
- **有限群性质**：  
(1)有限群$G$的任一子群$H$的阶为$G$的阶的因子，准确说：
$$|G|=|H|[G:H].$$  
(2)有限群$G$每个元素的阶是$G$的阶的因子。
- **素数阶群**：素数阶群一定为循环群。

### 8. 不变子群

*目标：*
掌握不变子群（正规子群）的定义，能掌握一个群的子群是不变子群（正规子群）的充分必要条件的定理，理解商群的定义，能证明一个群同它的每一个商群同态的定理，了解核的定义，掌握两个具有同态关系的群之间子群或不变子群（正规子群）的象的性质。并能将子群或不变子群（正规子群）的性质运用到循环群、变换群等群之中。

*内容：*

- **正规子群**：群$G$的子群$N$满足：任意$g\in G$，
$$gNg^{-1}=N,$$
称$N$是$G$的一个正规子群，记作$N\lhd G$.
- **共轭子群**：设$H$为群$G$的子群，对任意$g\in G$，$gHg^{-1}$也是$G$的子群，称$gHg^{-1}$为$H$的共轭子群。
- **等价条件**：群$G$的子群$H$是$G$的正规子群，等价于任意$a\in G$有$aH=Ha$.
- **群同态基本定理**：设$\sigma$为群$G$到$G'$的一个同态，则同态像同构于商群$G/Ker\sigma$,即
$$G/Ker \sigma \cong Im\sigma.$$
- **第一同构定理**：设$G$是群，$H$是$G$的子群，$N$是$G$的正规子群，则：  
(1)$HN$是$G$的子群；  
(2)$H\cap N$是$H$的正规子群，且$H/H\cap N\cong HN/N$.
- **第二同构定理**：设$G$为群，$H$和$N$都是$G$上正规子群，且$N\subset H$，则$H/N$为$G/N$的正规子群，且
$$(G/N)/(H/N)\cong G/H.$$
- **单群**：如果群$G$只有平凡的正规子群，则称$G$为单群。
- **换位子群(导群)**：称$xyx^{-1}y^{-1}$为$x$与$y$的换位子，记作$[x,y]$.群$G$的所有换位子生成的群称为$G$的换位子群，记作$[G,G]$,即
$$[G,G]=\langle\{xyx^{-1}y^{-1}|x,y\in G\}\rangle.$$
- **换位子群性质**：设$G'$是$G$的换位子群，则  
(1)$G'$是$G$的正规子群；  
(2)$G/G'$是Abel群，且若$N$是$G$的正规子群，有$G/N$为正规子群当且仅当$G'\subset N$.


### 9. sylow 定理

*目标：*
掌握 sylow 定理的应用。

*内容：*
- **sylow第一定理**：设群$G$的阶为$n=p^lm$，其中$p$为素数，$(m,p)=1$,$l>0$,则对于$1\le k \le l$，$G$中必有$p^k$阶子群，其中$p^l$阶子群（即$p$的最高幂阶子群）称为$G$的Sylow $p$-子群。
- **sylow第二定理**：设群$G$的阶为$n=p^lm$，其中$p$为素数，$(m,p)=1$,$l>0$,则  
(1)对于$1\le k \le l$,$G$的任意一个$p^{k}$阶子群一定包含在$G$的某一个Sylow $p$-子群中；  
(2)$G$的任意两个Sylow $p$-子群在$G$中共轭。
- **sylow第三定理**：设群$G$的阶为$n=p^lm$，其中$p$为素数，$(m,p)=1$,$l>0$,则$G$的Sylow $P$-子群的个数$r$模$p$同余$1$，并且$r$是$m$的因子。即
$$r \equiv 1 \pmod{p},\ \ \text{且} r|m.$$


## 三. 环与域

### 1. 交换环

*目标：*理解交换环的定义和例子，熟悉单位元、逆元和零因子的性质并能熟练运用。掌握消去律与零因子的关系。

*内容：*
- **环**：设$R$是一个非空集合，如果在$R$中有两种二元运算，对于其中一种运算(加法)成为交换群，对于另一种运算(乘法)成为半群，且满足分配律：
$$a(b+c)=ab+ac,\ (a+b)c=ac+bc,\ \ \forall a,b,c \in R,$$
则称$R$为一个环。
- **交换环**：如果对于环$R$的乘法还满足交换律，称$R$为交换环。
- **幺环**：如果对于环$R$的乘法存在单位元(记作$1$)，称$R$为幺环。
- **零因子**：设$a,b$是环$R$上的元素，且$a\neq 0,\ \ b\neq 0$，若$ab=0$，则称$a$($b$)为环$R$的一个左(右)零因子。
- **特征**：设环$R$为无零因子环，若$R$中所有非零元都是无穷阶的，则称$R$的特征为$0$，若$R$中所有非零元都是有限阶$p$阶($p$为素数)的，称$R$的特征为$p$。
- **消去律与零因子**：一个环$R$没有零因子，当且仅当$R$满足左右消去律。
- **无零因子环与阶**：设环$R\neq \{0\}$,且为无零因子环，则$R$中所有的非零元对于$R$的加法具有相同阶，且当这个共同阶为有限时，必为素数。
- **特征性质**：设无零因子交换环$R$的特征为$p$，$p$为素数，则
$$(a+b)^p=a^p+b^p,\ (a-b)^p=a^p-b^p,\ \ \forall a,b\in R.$$

### 2. 除环

*目标：*了解除环的定义，能举出域的例子，除环与加群、乘群的关系。熟悉无零因子环中的计算规则，掌握无零因子环中特征的性质。

*内容：*
- **除环**： 环$R$的所有非零元组成的集合对于乘法成一个群，称$R$为除环或者体。
- **域**：交换除环称为域。

### 3. 子环、子除环

*目标：*理解子环、子除环的定义，并能写出子整环、子域的概念，了解同态、同构环之间的性质，了解多项式成环，熟悉多项式环中的未定元、次数以及系数、无关未定元的作用。

*内容：*
- **子环**：如果环$R$的一个非空子集$R_1$对于$R$的加法和乘法也成环，则称$R_1$为$R$的一个子环。
- **子环充要条件**：设$R_1$为环$R$的非空子集，则$R_1$为$R$的子环的充要条件是对于任意$a,b\in R_1$，有$a-b\in R_1$，$ab\in R_1$;

### 4. 理想

*目标：*掌握理想的定义，理解理想的构成，以及零理想、单位理想和主理想的构成，能判断一个子环是否为理想，和理想是否为主理想。了解什么是最大理想，且和剩余类环的关联。

*内容：*
- **理想**：设环$R$的子环$I$满足
$$ar\in I,\ ra\in I,\ \ \forall a\in I,\forall r\in R.$$
则称$I$是$R$的一个理想。
- **由$S$生成的理想**：设$S$是环$R$的非空子集，环$R$包含$S$的所有理想的交集称为由$S$生成的理想。
- **零理想**：
- **单位理想**：
- **主理想**：环$R$由一个元素$a$生成的理想称为主理想，记作$(a)$，其实
$$(a)=\{r_1a+ar_2+ma+\sum_{i=1}^{n}x_iay_i|r_1,r_2,x_i,y_i\in R,m\in\mathbb{Z},n\in\mathbb{Z}^{+}\}.$$
- **互素**：设$R$是幺环，$I,J$是$R$的理想，如果$I+J=R$，则称$I$与$J$互素。
- **理想充要条件**：设$R_1$为环$R$的非空子集，则$R_1$为$R$的理想的充要条件是对于任意$a,b\in R_1$，$x,y\in R$，有$a-b\in R_1$，$xa,ay\in R_1$.
- **商环**：设$I$是环$R$的理想，$I$的所有陪集组成一个环，称为$R$对于$I$的商环，记作$R/I$.
- **环的同态**：设$\sigma$为环$R$到环$R'$的映射，且满足任意$a,b\in R$有
$$\sigma (a+b)= \sigma(a)+\sigma(b),$$
$$\sigma(ab)= \sigma(a)\sigma(b),$$
称$\sigma$是$R$到$R'$的同态。
- **环的同构**：设$\sigma$为环$R$到环$R'$的双射，且满足任意$a,b\in R$有
$$\sigma (a+b)= \sigma(a)+\sigma(b),$$
$$\sigma(ab)= \sigma(a)\sigma(b),$$
称$\sigma$是$R$到$R'$的同构。
- **环同态基本定理**：设$\sigma$为环$R$到环$R'$的同态，则同态像$Im \sigma$同构于商环$R/Ker \sigma$，即
$$R/Ker\sigma \cong Im \sigma.$$
- **素理想**：设$I$为环$R$的理想，如果由$ab\in I$，可推出$a\in I$或$b\in I$，则称$I$为$R$的一个素理想。
- **极大理想**：设$R$是交换幺环，$M$是$R$的理想，若$M\neq R$，且不存在$R$的真理想使得
$$M\subset N, M\neq N,$$
则称$M$为$R$的极大理想。

### 5. 无零因子的交换环

*目标：*掌握没有零因子的交换环一定是一个域的子环，了解商域的构成，并掌握同构的环的商域也同构的定理。理解主理想环的概念和引理，能证明主理想环是唯一分解环。

*内容：*
- **整除**：设$R$为一个整环，$a,b\in R$，若存在$c\in R$，使得$a=bc$，称$a$能被$b$整除，这时也称$b$为$a$的因子，记为$b\mid a$，若不能被$b$整除记为$b\nmid a$.
- **单位**：设$R$为整环，用$U$表示幺半群$R^{* }=R-\{0\}$中所有可逆元的集合，则$U$是一个交换群，称为$R$的单位群，$U$的元素称为单位。
- **相伴**：设$a,b\in R$，若存在$R$中单位$u$使得$a=ub$，则称$a$与$b$相伴，记为$a\sim b$
- **平凡因子和真因子**：设$R$为整环，$a\in R^{* }$，则任何单位和$a$的相伴元都是$a$的因子，称为$a$的平凡因子，若$b\mid a$，但$a\nmid b$，则称$b$为$a$的真因子。
- **可约元素**：设$R$为整环，$a\in R^{* }-U$，若$a$没有非平凡的真因子，则称$a$为不可约元素，若$a$有非平凡的真因子，则称$a$为可约元素。
- **素元素**：设$R$为整环，$p\in R^{* }-U$，且$p\mid ab$可推出$p\mid a$或$p\mid b$，则称$p$为素元素。(素元素一定是不可约元素。)
- **唯一分解环**：如果整环$R$满足：  
(1)有限分解条件：任意$a\in R^{* }-U$，$a$可分解为有限个不可约元素乘积，即存在不可约元素$p_i(1\le i\le r)$使得
$$a=p_1p_2\cdots p_r;$$  
(2)相伴意义下分解唯一：若$a\in R^{* }-U$有两种不可约元素乘积的分解：
$$a=p_1p_2\cdots p_s=q_1q_2\cdots q_r,$$
则有$r=s$，并且适当交换顺序可使得
$$p_i\sim q_i(1\le i\le r);$$
称$R$为唯一分解环。
- **公因子**：设$R$为整环，$a_1,a_2,\cdots, a_n\in R$，若$c$同时能够整除$a_1,a_2,\cdots,a_n$，则称$c$为$a_1,a_2,\cdots,a_n$的公因子，若$a_1,a_2,\cdots,a_n$的公因子$d$能够被$a_1,a_2,\cdots,a_n$的任何一个公因子整除，则称$d$为$a_1,a_2,\cdots,a_n$的一个最大公因子。

- **没有零因子的交换环一定是一个域的子环**
- **商域的构成**
- **同构的环的商域也同构的定理**
- **主理想环的概念和引理**
- **主理想环**：若交换幺环的每一个理想都是主理想，则称此环为主理想环。若一个主理想环是整环，则称此环为主理想整环。
- **证明主理想环是唯一分解环**

### 6. 欧氏环

*目标：*理解欧氏环的定义，理解欧氏环、整数环都是主理想环与唯一分解环的证明，并能证明域一定是一个欧氏环。

*内容：*
- **欧氏环**：设$R$为一个整环，若存在从$R^{* }$到$\mathbb{N}\cup \{0\}$的映射$\delta$，使得任意$a,b\in R,\ b\neq 0$，存在$q,r\in R$，满足
$$a=qb+r,$$
其中$r=0$，或$\delta(r)<\delta(b)$.称$R$为欧氏环(Euclid环)。
- **欧氏环是主理想环**：
- **欧氏环是唯一分解环**：
- **整数环是主理想环**：
- **整数环是唯一分解环**：
- **域一定是一个欧氏环**：