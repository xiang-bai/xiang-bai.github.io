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
## 几何与拓扑：代数拓扑、微分拓扑、流形与李群、黎曼几何
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

