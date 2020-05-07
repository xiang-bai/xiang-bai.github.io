---
layout: post
title:  "阿里巴巴数学竞赛2020决赛试题"
date:   2020-04-23 02:34:20 +0800
categories: math
tags: other
---

# 阿里巴巴数学竞赛2020决赛试题

* any list
{:toc}

## 代数与数论：群论、丢番图方程、伽罗华理论、代数数论、抽象代数、交换代数

1. 设$F$为域。考虑$F^n$上的如下环结构,加法是通常的向量加法,乘法定义为
 \begin{equation}
 \left(x_{1}, \ldots, x_{n}\right) \cdot\left(y_{1}, \ldots, y_{n}\right)=\left(x_{1} y_{1}, \ldots, x_{n} y_{n}\right)
 \end{equation}
 设 $\Lambda \subset F^{n}$ 为包含 $(1, \ldots, 1)$ 的子环。假设 $\Lambda$ 为整环, 而且它作为加法群是有限生成的。试证对于$\Lambda$的任何非零元$(x_1, \ldots, x_{n})$,我们有 $\prod_{i=1}^{n} x_{i} \neq 0$.
2. 设群$G$作用在集合$\Omega$上,使得所有$G$-轨道都是无限集。设$\Gamma, \Delta$为$\Omega$的有限子集。试证存在$g \in G$使得$g \Gamma\cap\Delta=\varnothing$.
3. 设$V$为域$F$上的有限维向量空间, $\operatorname{char}(F) \neq 2$, 令$q: V \to F$为二次型,也就是说:存往对称$F$-双线性型$B : V^{2} \to F$(必然唯一)使得$q(v)=B(v, v)$对所有$v$成立。对所有域扩张$F\hookrightarrow E$,定义二次型$q$到$E$上的基变换为
 \begin{equation}
 q_{E}: E \otimes_{F} V \rightarrow E ; \quad q_{E}(a \otimes v)=a^{2} q(v), \quad a \in E, v \in V
 \end{equation}
 我们说$q$是迷向的,如果$v \neq 0 \Longleftrightarrow q(v) \neq 0$
 (a) 试证如果$q$迷向,而$[E: F]$是奇数,那么 $q_{E}$ 也是迷向的。
 (b) 以上叙述在$[E: F]$为偶数时是否成立?
4. 找出所有满足以下条件的有限群$G$：
 - $G$的阶是相异素数的积,换句话说,存往相异素数$p_{1}, \ldots, p_{m}$使得$\sharp G=p_{1} \cdots p_{m}$
 - $G$的所有非平凡元都是素数阶的,换句话说每个元素的阶数都属于$\{1, p_{1}, \ldots, p_{m}\}$    
 (注记:答案和$m$有关;例如当$m=2$时存在许多这样的$G$;您必须对它们分类。)
5. 找出所有$(k, \alpha)$,其中$k>2$是整数而$\alpha \neq 0$是复数,使得
 \begin{equation}
 \alpha \in\{r e^{\frac{i \pi}{k}} \mid r \in \mathbb{R}\}, \quad \alpha+\alpha^{-1} \in\{m+n \sqrt{-2}\mid m, n \in \mathbb{Z}\}.
 \end{equation}



## 几何与拓扑：代数拓扑、微分拓扑、流形与李群、黎曼几何

6. 设$S_{g}$是亏格为$g$的可定向闭曲面,$N_{2 g}$是亏格为$2 g$的不可定向闭曲面(即$N_{2 g}$由球面粘接$2 g$个“交叉帽”得到). 设$f: N_{2 g} \to S_{g}$是连续映射. 证明：诱导映射$f_{* }: H_{2}(N_{2 g} ; \mathbb{Z} / 2 \mathbb{Z}) \to H_{2}(S_{g} ; \mathbb{Z} / 2 \mathbb{Z})$ 恒为$0$.
7. 设$S^{3}$是$\mathbb{R}^{4}$中的单位球面，赋予标淮的李群结构，$x$为 de Rham 上同调$H^{3}(S^{3}, \mathbb{R})$的一个非零元. 证明：不存在李群同构$f: S^{3} \to S^{3}$使得 $f^{* }(x)=-x$.
8. 设$\mathbb{C}P^2$为复射影平面, $L_{1}, L_{2}, L_{3}$为其中三条复射影直线，满足 $L_{1} \cap L_{2}\cap L_{3}=\varnothing$. 取$L_{1}, L_{2}, L_{3}$各自的紧致管状邻域，使得它们的并是一个(实)4维带边紧致流形$W$，边界记为$M = \partial W$, 并且要求$W \backslash (L_{1} \cup L_{2} \cup L_{3})$同胚于$M \times[0,1) $. 请计算$M$的$\mathbb{Z}$系数同调群.
9. 设$(M,g)$是$n$维黎曼流形$(n \geq 3)$, 截面曲率$K \geq 0$. 设$\gamma(t)$为测地线, $t \in[0, T)$, 其中$t$是弧长参数. 假设$J_{1}, \ldots, J_{n-1}$是沿$\gamma$的Jacobi场, 都垂直于$\gamma^{\prime}$, 且在每一点都线性无关。假设对任何$i, j$都满足
 \begin{equation}
 (J_{i}^{\prime}(0), J_{j}(0))=(J_{i}(0), J_{j}^{\prime}(0))
 \end{equation}
 其中$J_{i}^{\prime}$表示$J_{i}$沿$\gamma^{\prime}$方向的协变导数。证明: 对每个$i=1, \ldots, n-1$和$0< s< t<T$, 都有$\frac{\vert J_{i}(s)\vert_{g}}{s} \geq \frac{\vert J_{i}(t)\vert_{g}}{t}$.
10. 设$M$是$5$维紧致光滑流形$SO(3) \times T^2$，其中$T^{2}$为一个$2$维环面.   
 (1) 是否存在$M$上的光滑黎曼度量$g$使得Ricci曲率严格为正?    
 (2) 是否存在$M$上的光滑黎曼度量$g$ 使得$Ric \equiv 0 $?    
 如果存在请给出具体的例子，如果不存在请给出证明.   



## 分析与方程：实分析、调和分析、偏微分方程

11. 假设$g(x)$是定义在$\mathbb{R}^{3}$上的光滑Schwarz函数（也称速降函数），满足条件
\begin{equation}
\int_{\vert y\vert=1} g(x+y) d \sigma(y)=0, \quad \forall x \in \mathbb{R}^{3}
\end{equation}
这里$d\sigma(y)$是球面$\{\vert y\vert = 1 \}$上的标准面积单元。证明$g = 0$.

12. 假设$\mathbb{R}^3$上的球对称函数$u(x)$(也就是当$\vert x\vert = \vert y\vert$时有$u(x) = u(y)$)满足方程
\begin{equation}
\Delta u-u+\vert u\vert ^{2} u=0, \quad \forall x \in \mathbb{R}^{3}
\end{equation}
如果$u\in C^2(\mathbb{R}^3)\bigcap H^{1}(\mathbb{R}^3)$，证明存在常数$C$使得
\begin{equation}
\vert u(x)\vert \leq C e^{-\frac{1}{2}\vert x\vert}
\end{equation}

13. 考虑限$\mathbb{R}^n$中的有界区域$\Omega$，以及定义在这个区域上的非负函数$\kappa$使得对常数 $\alpha>1, M>0, E_{0}>0 $有
\begin{equation}
M \leq \int_{\Omega} \kappa d x, \quad \int_{\Omega} \kappa^{\alpha} d x \leq E_{0}
\end{equation}
证明存在只依赖于$M, E_0, \alpha$的常数$C$使得
\begin{equation}
\Vert v\Vert_{L^{2}(\Omega)} \leq C\left(\Vert \nabla v\Vert_{L^{2}(\Omega)}+\int_{\Omega} \kappa|v| d x\right), \quad \forall v \in H^{1}(\Omega)
\end{equation}

14. 在$\mathbb{R}^n$上考虑薛定谔方程
\begin{equation}
i \partial_{t} u+\Delta u=0, \quad u(0, x)=u_{0}(x), \quad x \in \mathbb{R}^{n}
\end{equation}
假设初始值 $u_{0} \in L^{2}\left(\mathbb{R}^{n}\right)$.证明
\begin{equation}
\lim _ {T \rightarrow \infty} \frac{1}{T} \int_{0}^{T} \int_{|x| \leq \sqrt{t}}|u(t, x)|^{2} d x d t=0
\end{equation}

15. 考虑标准的2维环面$\mathbb{T}^2 = \mathbb{R}^2/\mathbb{Z}^2$, 以及上面的半径为$0.1$的圆圈$S$。证明存在常数$C>0$使得对任意定义在环面上，并且满足方程
\begin{equation}
\partial_{x_{1}}^{2} f-\partial_{x_{2}}^{2} f=\lambda f, \quad \lambda \neq 0
\end{equation}
的函数$f$均满足不等式 
\begin{equation}
\Vert f\Vert_{L^{2}(S, \mathrm{d} s)} \leq C\Vert f\Vert_{L^{2}\left(\mathbb{T}^{2}\right)}.
\end{equation}
其中$ds$为圆圈的弧长测度。

## 应用与计算数学：组合数学、图论、概率、优化理论、常微分方程、偏微分方程、数值分析

16. 一个简单图$G$称为“漂亮的”, 如果它的任意两个相邻顶点的度数不同. 对任意$n \geq 2$, 定义$f(n)$为$n$阶“漂亮的”简单图的边数的最大值. 求满足
 \begin{equation}
 \lim_{n \to \infty} \frac{\tbinom{n}{2}-f(n)}{n^{a}}=b
 \end{equation}
 的实数 $a, b \quad(b \neq 0)$.
17. 令$a$和$b$为两个正整数, 在一个不透明的袋子里放了$a$个红球和$b$个蓝球. 红球和蓝球除了颜色以外的其它特征相同, 只能通过颜色来分辨. 小明进行如下的游戏: 每一轮她从袋子里随机抽取一个球, 如果这个球是蓝球, 那么游戏结束：如果是红球, 那么她将该球放回袋子并再加放一个红球到袋子之中（这样袋子中的红球增多了一个）. 令$E_{a, b}$为游戏总轮数的期望.   
 (1) 当$a$与$b$为何值时, 期望$E_{a, b}$取有限值?   
 (2) 将$E_{a, b}$表示为$a$与$b$的函数.   
 (3) 假设小明知道袋中的总球数$N$但不知道$a$与$b$的值. 她先验地认为$a$在集合$\{1, \ldots, N-1\}$中均匀分布. 在第几轮抽到红球的情况下她可以有$90%$的把握猜测$E_{a, b}$取无穷值?
18. 给定$n$个正实数$a_{1}, \cdots, a_{n}$, 假设它们满足$a_{1}^{2}+\cdots+a_{n}^{2}=1$和$a_{1}+\cdots+a_{n}=a$. 证明 存在一种挑选系数 $\epsilon_{1}, \cdots \epsilon_{n}$ 的方法，使得每个系数 $\epsilon_{i}$ 均为 $1$ 或 $-1$, 并且
 \begin{equation}
 \vert \epsilon_{1} a_{1}+\cdots+\epsilon_{n} a_{n}\vert \leq \frac{1}{a}
 \end{equation}
 比如当$n=5$且$a_{1}=\cdots=a_{5}=1 / \sqrt{5}$时$a=\sqrt{5}$, 可以取$\epsilon_{1}=\epsilon_{2}=\epsilon_{3}=1, \epsilon_{4}=\epsilon_{5}=-1$, 
 这样$\vert \epsilon_{1} a_{1}+\cdots+\epsilon_{5} a_{5}\vert = 1 / \sqrt{5}=1 / a$.
19. 在分子动力学中, 人们常使用 overdamped Langevin equation
 \begin{equation}
 \dot{x}=f(x)+\sqrt{2 \beta^{-1}} \eta
 \end{equation}
 来采样 Boltzmann 分布 $\rho_{\beta}(x)=Z_{\beta}^{-1} e^{-\beta V(x)}$, 这里 $x \in \mathbb{R}^{3 n}, \beta=\frac{1}{k_{\beta} T}>0$, $k_{B}$是Boltzmann 常数, $T$是温度, $f(x)=-\nabla V(x)$ 是由势函数$V(x)$决定的作用力, $\eta$是一个$3 \mathrm{n}$维的白噪声, 而$Z_{\beta}=\int_{\mathrm{R}^{3n}} e^{-\beta V(x)} d x$ 是归一化常数. 考虑如下的两条耦合的采样轨道,
 \begin{equation}
 \begin{cases}
 \dot{x}_ {1}=f(x_{1})+\sqrt{2 \beta_{1}^{-1}(t)} \eta_{1} \newline
 \dot{x}_ {2}=f(x_{2})+\sqrt{2 \beta_{2}^{-1}(t)} \eta_{2}
 \end{cases}
 \end{equation}
 其中$\beta_{1}(t)$和$\beta_{2}(t)$会交替地取值$\beta>0$和$\bar{\beta}>0$. 例如, 可选 $\bar{\beta}<\beta$  (即 $\bar{\beta}^{-1}>\beta^{-1}$) 使得$\bar{\beta}$对应的温度高于原系统的温度以提高采样效率. 按照频率$\nu, \beta_{1}(t)$和$\beta_{2}(t)$会尝试互换取值, 如界互换是尝试从$(\beta_{1}, \beta_{2})=(\beta, \bar{\beta})$变成$(\beta_{1}, \beta_{2})=(\bar{\beta}, \beta)$, 那么这种互换的接受概率为
 \begin{equation}
 \min \left(\frac{\rho_{\bar{\beta}}(x_{1}) \rho_{\beta}(x_{2})}{\rho_{\beta}(x_{1}) \rho_{\bar{\beta}}(x_{2})}, 1\right)\ \ (1)
 \end{equation}
 而另外一种互换的接受概率类似可得. 写出（无需证明）当频率$\nu \to \infty$时$(1)$的极限方程, 我们称之为系统（A）. 写出另一个$x_1$和$x_{2}$满足的随机动力方程, 我们称之为系统（B），使得系统（B）中只含有常系数的噪声项, 且系统（A）和系统（B）对应一样的不变分布。
20. 假设 $x_{1}, \ldots, x_{n}$ 是一组相异实数, $y_{1}, \ldots, y_{n}$是另一组相异实数, 并且对于每个$i=1, \ldots, n$都有$y_{i} \geq x_{i}$. 一个单向运输$T$是一个从$\{x_{1}, \ldots, x_{n}\}$到$\{y_{1}, \ldots, y_{n}\}$的一一映射，并且满足对于每个$i=1, \ldots, n$都有$T(x_{i}) \geq x_{i}$. (例如, 对每个$i=1, \ldots, n$使$T(x_{i})=y_{i}$就定义了一个单向运输.) $T$的运输成本定义为
 \begin{equation}
 \sum_{i=1}^{n}(T(x_{i})-x_{i})^{2}
 \end{equation}
 (1) 找到或描述分别最小化和最大化运输成本的两个单向运输，并证明它们的最优性.
 (2) 假设$(x_{n})_ {n=1,2,\ldots}$, 是一列来自标准正态分布的独立同分布序列, 并且$y_{i}=x_{i}+1$, $i=1,2, \ldots $. 令$T_{n}^{* }$为从$X_{n}:=\{x_{1}, \ldots, x_{n}\}$到$Y_{n}:=\{y_{1}, \ldots, y_{n}\}$ 的最大化运输成本的单向运输. 计算以下随机量
 \begin{equation}
 \frac{\sharp \{x \in X_{n}: x \leq 0, T_{n}^{* }(x) \leq 1\}}{n}
 \end{equation}
 当$n \to \infty$时的极限(在几乎必然(a.s.)意义下),其中$\sharp$表示集合的势.

## <a href="http://www.13ai.club/images/ali-math-competition-2020.pdf" download>PDF下载</a>
 