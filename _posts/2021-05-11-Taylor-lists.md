---
layout: post
title:  "常用Taylor级数"
date:   2021-05-11 02:34:20 +0800
categories: math
tags: other
---

# 常用Taylor级数

* any list
{:toc}

\begin{equation}
\begin{array}{l}
e^{x}=\sum_{n=0}^{\infty} \frac{1}{n !} x^{n}=1+x+\frac{1}{2 !} x^{2}+\cdots+\frac{1}{n !} x^{n}+\cdots, x \in(-\infty,+\infty)\newline
\sin x=\sum_{p=0}^{\infty} \frac{(-1)^{n}}{(2 n+1) !} x^{2 x+1}=x-\frac{1}{3 !} x^{3}+\frac{1}{5 !} x^{5}-\cdots+\frac{(-1)^{n}}{(2 n+1) !} x^{2 n+1}+\cdots, x \in(-\infty,+\infty)\newline
\cos x=\sum_{n=0}^{\infty} \frac{(-1)^{n}}{(2 n) !} x^{2 n}=1-\frac{1}{2 !} x^{2}+\frac{1}{4 !} x^{4}-\cdots+\frac{(-1)^{n}}{(2 n) !} x^{2 n}+\cdots, x \in(-\infty,+\infty)\newline
\ln (1+x)=\sum_{n=0}^{\infty} \frac{(-1)^{n}}{n+1} x^{n+1}=x-\frac{1}{2} x^{2}+\frac{1}{3} x^{3}-\cdots+\frac{(-1)^{n}}{n+1} x^{n+1}+\cdots, x \in(-1,1]\newline
\frac{1}{1-x}=\sum_{p=0}^{\infty} x^{n}=1+x+x^{2}+x^{3}+\cdots+x^{n}+\cdots, x \in(-1,1)\newline
\frac{1}{1+x}=\sum_{x=0}^{\infty}(-1)^{n} x^{n}=1-x+x^{2}-x^{3}+\cdots+(-1)^{n} x^{n}+\cdots, x \in(-1,1)\newline
(1+x)^{\alpha}=1+\sum_{n=1}^{\infty} \frac{\alpha(\alpha-1) \cdots(\alpha-n+1)}{n !} x^{n}=1+\alpha x+\frac{\alpha(\alpha-1)}{2 !} x^{2}+\cdots+\frac{\alpha(\alpha-1) \ldots(\alpha-n+1)}{n !} x^{n}+\cdots, x \in(-1,1)\newline
\arctan x=\sum_{n=0}^{\infty} \frac{(-1)^{n}}{2 n+1} x^{2 n+1}=x-\frac{1}{3} x^{3}+\frac{1}{5} x^{5}+\cdots+\frac{(-1)^{n}}{2 n+1} x^{2 n+1}+\cdots, x \in[-1,1]\newline
\arcsin x=\sum_{n=0}^{\infty} \frac{(2 n) !}{4^{\pi}(n !)^{2}(2 n+1)} x^{2 p+1}=x+\frac{1}{6} x^{3}+\frac{3}{40} x^{5}+\frac{5}{112} x^{7}+\frac{35}{1152} x^{9}+\cdots+\frac{(2 n) !}{4^{n}(n !)^{2}(2 n+1)} x^{2 n+1}+\cdots, x \in(-1,1)\newline
\tan x=\sum_{n=1}^{\infty} \frac{B_{2 n}(-4)^{n}\left(1-4^{n}\right)}{(2 n) !} x^{2 n-1}=x+\frac{1}{3} x^{3}+\frac{2}{15} x^{5}+\frac{17}{315} x^{7}+\frac{62}{2835} x^{9}+\frac{1382}{155925} x^{11}+\frac{21844}{6081075} x^{13}+\frac{929569}{638512875} x^{15}+\cdots x \in(-1,1)\newline
\sec x=\sum_{n=0}^{\infty} \frac{(-1)^{n} E_{2 n} x^{2 n}}{(2 n) !}=1+\frac{1}{2} x^{2}+\frac{5}{24} x^{4}+\frac{61}{720} x^{6}+\cdots, x \in\left(-\frac{\pi}{2}, \frac{\pi}{2}\right)\newline
\csc x=\sum_{n=0}^{\infty} \frac{(-1)^{n+1} 2\left(2^{2 n-1}-1\right) B_{21}}{(2 n) !} x^{2 x-1}=\frac{1}{x}+\frac{1}{6} x+\frac{7}{360} x^{3}+\frac{31}{15120} x^{5}+\frac{127}{604800} x^{7}+\frac{73}{3421440} x^{9}+\frac{1414477}{65383718400} x^{11}+\cdots, x \in(0, \pi)\newline
\cot x=\sum_{\pi=0}^{\infty} \frac{(-1)^{n} 2^{2 n} B_{2 n}}{(2 n) !} x^{2 n-1}=\frac{1}{x}-\frac{1}{3} x-\frac{1}{45} x^{3}-\frac{2}{945} x^{5}-\cdots, x \in(0, \pi)\newline
\text { sh } x=\sum_{n=0}^{\infty} \frac{x^{2 n+1}}{(2 n+1) !}=x+\frac{x^{3}}{3 !}+\frac{x^{5}}{5 !}+\frac{x^{7}}{7 !}+\cdots+\frac{x^{20+1}}{(2 n+1) !}+\cdots, x \in(-\infty,+\infty)\newline
\text { ch } x=\sum_{j=0}^{\infty} \frac{x^{2 n}}{(2 n) !}=1+\frac{x^{2}}{2 !}+\frac{x^{4}}{4 !}+\frac{x^{6}}{6 !}+\cdots+\frac{x^{2 n}}{(2 n) !}+\cdots, x \in(-\infty,+\infty)\newline
\text { th } x=\sum_{n=1}^{\infty} \frac{2^{20}\left(2^{2 n}-1\right) B_{2 \pi} x^{2 n-1}}{(2 n) !}=x-\frac{1}{3} x^{3}+\frac{2}{15} x^{3}-\frac{17}{315} x^{7}+\frac{62}{2835} x^{9}-\frac{1382}{155925} x^{11}+\cdots,|x|<\frac{\pi}{2}\newline
\operatorname{arsh} x=\sum_{x=0}^{\infty}\left(\frac{(-1)^{n}(2 n) !}{2^{24}(n !)^{2}}\right) \frac{x^{20+1}}{(2 n+1)}=x-\frac{1}{6} x^{3}+\frac{3}{40} x^{5}-\frac{5}{112} x^{7}+\frac{35}{1152} x^{9}-\cdots+\left(\frac{(-1)^{n}(2 n) !}{2^{20}(n !)^{2}}\right) \frac{x^{2 n+1}}{(2 n+1)}+\cdots,|x|<1\newline
\operatorname{arch} x=\ln 2 x-\sum_{n=1}^{\infty}\left(\frac{(-1)^{n}(2 n) !}{2^{2 n}(n !)^{2}}\right) \frac{x^{-2 n}}{2 n}=\ln 2 x-\left(\frac{1}{4} x^{-2}+\frac{3}{32} x^{-4}+\frac{15}{288} x^{-6}+\cdots+\left(\frac{(-1)^{n}(2 n) !}{2^{2 H}(n !)^{2}}\right) \frac{x^{-2 n}}{2 n}+\cdots\right),|x|>1\newline
\text { arthx }=\sum_{n=0}^{\infty} \frac{x^{2 n+1}}{2 n+1}=x+\frac{x^{3}}{3}+\frac{x^{5}}{5}+\frac{x^{7}}{7}+\cdots+\frac{x^{2 n+1}}{2 n+1}+\cdots,|x|<1
\end{array}
\end{equation}