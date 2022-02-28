---
layout: post
title:  "Taylor’s formula"
date:   2022-02-22 02:34:20 +0800
categories: math
tags: other
---

# Taylor’s formula

* any list
{:toc}

Taylor 公式
\begin{equation}
f(x+h)=\sum_{\vert\alpha\vert \leq k} \frac{\partial^{\alpha} f(x)}{\alpha !} h^{\alpha}+R(h, x, k)
\end{equation}
其中余项 $R(h, x, k)$ 可用 Langrange 均值形式
\begin{equation}
R(h, x, k)=\sum_{\vert\alpha\vert=k+1} \frac{\partial^{\alpha} f(x+c h)}{\alpha !} h^{\alpha} \quad \text{for some } c \in(0,1),
\end{equation}
或者积分形式
\begin{equation}
R(h, x, k)=(k+1) \sum_{\vert\alpha\vert=k+1} \frac{h^{\alpha}}{\alpha !} \int_{0}^{1}(1-t)^{k} \partial^{\alpha} f(x+t h) d t
\end{equation}
