---
layout: post
title:  "Leibniz Rule"
date:   2022-02-22 02:34:20 +0800
categories: math
tags: other
---

# Leibniz Rule(Leibniz 法则)

* any list
{:toc}

一维：    
\begin{equation}
\frac{d^{m}}{d t^{m}}(f g)=\sum_{k=0}^{m}\left(\begin{array}{l}
m \\
k
\end{array}\right) \frac{d^{k} f}{d t^{k}} \frac{d^{m-k} g}{d t^{m-k}}
\end{equation}
高维：    
\begin{equation}
\partial^{\alpha}(f g)=\sum_{\beta \leq \alpha}\left(\begin{array}{c}
\alpha_{1} \\
\beta_{1}
\end{array}\right) \cdots\left(\begin{array}{c}
\alpha_{n} \\
\beta_{n}
\end{array}\right)\left(\partial^{\beta} f\right)\left(\partial^{\alpha-\beta} g\right)
\end{equation}
