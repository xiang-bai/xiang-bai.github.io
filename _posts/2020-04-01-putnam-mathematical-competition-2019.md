---
layout: post
title:  "Putnam数学竞赛题目和解答2019"
date:   2020-04-01 02:34:20 +0800
categories: math
tags: other
---

# Putnam数学竞赛题目和解答2019

* any list
{:toc}

## A 部分
1. Determine all possible values of the expression
 \begin{equation}
 A^3+B^3+C^3-3ABC
 \end{equation}
 where $A, B$, and $C$ are nonnegative integers.

2. In the triangle $\triangle ABC$, let $G$ be the centroid, and let $I$ be the center of the inscribed circle.
 Let $\alpha$ and $\beta$ be the angles at the vertices $A$ and $B$, respectively.
 Suppose that the segment $IG$ is parallel to $AB$ and that $\beta = 2 \tan^{-1} (1/3)$. Find $\alpha$.

3. Given real numbers $b_0, b_1, \dots, b_{2019}$ with $b_{2019} \neq 0$, let $z_1,z_2,\dots,z_{2019}$ be 
 the roots in the complex plane of the polynomial 
 \begin{equation}
 P(z) = \sum_{k=0}^{2019} b_k z^k.
 \end{equation}
 Let $\mu = (|z_1| + \cdots + |z_{2019}|)/2019$ be the average of the distances from $z_1,z_2,\dots,z_{2019}$ to the origin. Determine the largest constant $M$ such that $\mu \geq M$ for all choices of $b_0,b_1,\dots, b_{2019}$ that satisfy
 \begin{equation}
 1 \leq b_0 < b_1 < b_2 < \cdots < b_{2019} \leq 2019.
 \end{equation}

4. Let $f$ be a continuous real-valued function on $\mathbb{R}^3$. Suppose that for every sphere $S$ of radius 1,
 the integral of $f(x,y,z)$ over the surface of $S$ equals 0. Must $f(x,y,z)$ be identically 0?
 
5. Let $p$ be an odd prime number, and let $\mathbb{F}_ p$ denote the field of integers modulo $p$. Let $\mathbb{F}_ p[x]$ be the ring of polynomials over $\mathbb{F}_ p$, and let $q(x) \in \mathbb{F}_ p[x]$ be given by 
 \begin{equation}
 q(x) = \sum_{k=1}^{p-1} a_k x^k,
 \end{equation}
 where
 \begin{equation}
 a_k = k^{(p-1)/2} \mod{p}. 
 \end{equation}
 Find the greatest nonnegative integer $n$ such that $(x-1)^n$ divides $q(x)$ in $\mathbb{F}_ p[x]$.

6. Let $g$ be a real-valued function that is continuous on the closed interval $[0,1]$ and twice differentiable on 
 the open interval $(0,1)$. Suppose that for some real number $r>1$, 
 \begin{equation}
 \lim_{x \to 0^+} \frac{g(x)}{x^r} = 0.
 \end{equation}
 Prove that either
 \begin{equation}
 \lim_{x \to 0^+} g'(x) = 0 \qquad \mbox{or} \qquad \limsup_{x \to 0^+} x^r |g''(x)| = \infty.
 \end{equation}

## B 部分

1. Denote by $\mathbb{Z}^2$ the set of all points $(x,y)$ in the plane with integer coordinates. For each integer $n \geq 0$, let $P_n$ be the subset of $\mathbb{Z}^2$ consisting of the point $(0,0)$ together with all points $(x,y)$ such that $x^2 + y^2 = 2^k$ for some integer $k \leq n$. Determine, as a function of $n$, the number of four-point subsets of $P_n$ whose elements are the vertices of a square.

2. For all $n \ge 1$, let
 \begin{equation}
 a_n=\sum_{k=1}^{n-1}\frac{\sin{(\frac{(2k-1)\pi}{2n})}}{\cos^2{(\frac{(k-1)\pi}{2n})}\cos^2{(\frac{k\pi}{2n})}}.
 \end{equation}
 Determine
 \begin{equation}
 \lim_{n\to \infty}\frac{a_n}{n^3}.
 \end{equation}
 **解**：由三角函数基本公式有
 \begin{equation}
 \begin{aligned}
 \cos^2{(\frac{(k-1)\pi}{2n})}-\cos^2{(\frac{k\pi}{2n})}=&\frac{1}{2}\big{(}\cos{(\frac{2(k-1)\pi}{2n})}-\cos{(\frac{2k\pi}{2n})}\big{)}\newline
 =&-\sin{(\frac{(2k-1)\pi}{2n})}\sin{(\frac{\pi}{2n})},
 \end{aligned}
 \end{equation}
 从而可知
 \begin{equation}
 \frac{\sin{(\frac{(2k-1)\pi}{2n})}}{\cos^2{(\frac{(k-1)\pi}{2n})}\cos^2{(\frac{k\pi}{2n})}}=-\frac{1}{\sin{(\frac{\pi}{2n})}}\Big{(}\frac{1}{\cos^2{(\frac{(k-1)\pi}{2n})}}-\frac{1}{\cos^2{(\frac{k\pi}{2n})}}\Big{)}.
 \end{equation}
 代入$a_n$得到
 \begin{equation}
 a_n=-\frac{1}{\sin{(\frac{\pi}{2n})}}\Big{(}1-\frac{1}{\cos^2(\frac{(n-1)\pi}{2n})}\Big{)}=-\frac{1}{\sin{(\frac{\pi}{2n})}}+\frac{1}{\sin^3{(\frac{\pi}{2n})}}.
 \end{equation}
 下面来求极限
 \begin{equation}
 \lim_{n\to \infty}\frac{a_n}{n^3}=\lim_{n\to \infty}\Big{(}-\frac{1}{n^3\sin{(\frac{\pi}{2n})}}+\frac{1}{n^3\sin^3{(\frac{\pi}{2n})}}\Big{)}=\frac{8}{\pi^3}.
 \end{equation}

3. Let $Q$ be an $n$-by-$n$ real orthogonal matrix, and let $u \in \mathbb{R}^n$ be a unit column vector (that is,
 $u^T u = 1$). Let $P = I - 2uu^T$, where $I$ is the $n$-by-$n$ identity matrix. Show that if $1$ is not an eigenvalue of $Q$, then $1$ is an eigenvalue of $PQ$.

4. Let $\mathcal{F}$ be the set of functions $f(x, y)$ that are twice continuously differentiable for $x \geq 1$,$y \geq 1$ and that satisfy the following two equations (where subscripts denote partial derivatives):
 \begin{equation}
 \begin{array}{c}
 x f_{x}+y f_{y}=x y \ln (x y) ,\newline
 x^{2} f_{x x}+y^{2} f_{y y}=x y.
 \end{array}
 \end{equation}
 For each $f \in \mathcal{F},$ let
 \begin{equation}
 m(f)=\min_ {s \geq 1}(f(s+1, s+1)-f(s+1, s)-f(s, s+1)+f(s, s)).
 \end{equation}
 Determine $m(f)$, and show that it is independent of the choice of $f$.    
 **解**：由$x f_{x}+y f_{y}=x y \ln (x y)$可得
 \begin{equation}
 x f_{xx}+f_{x}+ y f_{xy}=y \ln (x y) + y,\ \ (1)，
 \end{equation}
 和
 \begin{equation}
 y f_{yy} + f_{y} + x f_{xy}=x \ln (x y) + x,\ \ (2).
 \end{equation}
 然后$(1)* x+(2) * y$得到
 \begin{equation}
 2xy f_{xy} +x^2 f_{xx}+y^2 f_{yy} +xf_{x} + yf_{y} =2xy \ln (x y) + 2xy.
 \end{equation}
 带入题设的条件有
 \begin{equation}
 2f_{xy} =\ln (x y) + 1=\ln (x)+\ln (y)+1.
 \end{equation}
 下面来求目标函数，
 \begin{equation}
 \begin{aligned}
 F(s) \triangleq &f(s+1, s+1)-f(s+1, s)-f(s, s+1)+f(s, s)\newline
 = &\int_{s}^{s+1}f_{y}(s+1,y)-f_{y}(s,y)dy \newline
 = &\int_{s}^{s+1}\int_{s}^{s+1}f_{xy}(x,y)dxdy
 = \frac{1}{2}\int_{s}^{s+1}\int_{s}^{s+1} \ln (x) +\ln (y)+ 1dxdy\newline
 = & \int_{s}^{s+1} \ln (x )dx+\frac{1}{2}.
 \end{aligned}
 \end{equation}
 明显函数$F(s)$单调递增，故在$s=1$处取得最小值，即
 \begin{equation}
 m(s) =2\ln (2)-\frac{1}{2}.
 \end{equation}

5. Let $F_m$ be the $m$th Fibonacci number, defined by $F_1 = F_2 = 1$ and $F_m = F_{m-1} + F_{m-2}$ for all $m \geq 3$.
 Let $p(x)$ be the polynomial of degree $1008$ such that $p(2n+1) = F_{2n+1}$ for $n=0,1,2,\dots,1008$. Find integers $j$ and $k$ such that $p(2019) = F_j - F_k$.

6. Let $\mathbb{Z}^n$ be the integer lattice in $\mathbb{R}^n$. Two points in $\mathbb{Z}^n$ are called 
 *neighbors* if they differ by exactly $1$ in one coordinate and are equal in all other coordinates. 
 For which integers $n \geq 1$ does there exist a set of points $S \subset \mathbb{Z}^n$ satisfying the following two conditions?
 1. If $p$ is in $S$, then none of the neighbors of $p$ is in $S$.
 2. If $p \in \mathbb{Z}^n$ is not in $S$, then exactly one of the neighbors of $p$ is in $S$.
