---
layout: post
title:  "积分公式表"
date:   2020-04-26 02:34:20 +0800
categories: math
tags: other
---

# 积分公式表

* any list
{:toc}

## 含有$ax+b$的积分
\begin{equation} \int \ (ax+b)^{n}{\mbox{d}}x={\frac {(ax+b)^{n+1}}{a(n+1)}}+C\end{equation}\begin{equation} \int \ (ax+b)^{n}{\mbox{d}}x={\frac {(ax+b)^{n+1}}{a(n+1)}}+C\end{equation}
\begin{equation} \int {\frac {1}{ax+b}}{\mbox{d}}x={\frac {1}{a}}\ln \left\vert ax+b\right\vert+C\end{equation}\begin{equation} \int {\frac {1}{ax+b}}{\mbox{d}}x={\frac {1}{a}}\ln \left\vert ax+b\right\vert+C\end{equation}
\begin{equation} \int {\frac {x}{ax+b}}{\mbox{d}}x={\frac {1}{a^{2}}}(ax+b-b\ln \left\vert ax+b\right\vert)+C\end{equation}\begin{equation} \int {\frac {x}{ax+b}}{\mbox{d}}x={\frac {1}{a^{2}}}(ax+b-b\ln \left\vert ax+b\right\vert)+C\end{equation}
\begin{equation} \int {\frac {x^{2}}{ax+b}}{\mbox{d}}x={\frac {1}{2a^{3}}}\left[(ax+b)^{2}-4b(ax+b)+2b^{2}\ln \left\vert ax+b\right\vert\right]+C\end{equation}\begin{equation} \int {\frac {x^{2}}{ax+b}}{\mbox{d}}x={\frac {1}{2a^{3}}}\left[(ax+b)^{2}-4b(ax+b)+2b^{2}\ln \left\vert ax+b\right\vert\right]+C\end{equation}
\begin{equation} \int {\frac {1}{x(ax+b)}}{\mbox{d}}x=-{\frac {1}{b}}\ln \left\vert {\frac {ax+b}{x}}\right\vert+C\end{equation}\begin{equation} \int {\frac {1}{x(ax+b)}}{\mbox{d}}x=-{\frac {1}{b}}\ln \left\vert {\frac {ax+b}{x}}\right\vert+C\end{equation}
\begin{equation} \int {\frac {1}{x^{2}(ax+b)}}{\mbox{d}}x={\frac {a}{b^{2}}}\ln \left\vert {\frac {ax+b}{x}}\right\vert-{\frac {1}{bx}}+C
\end{equation}
\begin{equation} 
\int {\frac {1}{x^{2}(ax+b)}}{\mbox{d}}x={\frac {a}{b^{2}}}\ln \left\vert {\frac {ax+b}{x}}\right\vert-{\frac {1}{bx}}+C
\end{equation}

## 含有$\sqrt{a+bx}$的积分
\begin{equation} \int x{\sqrt {a+bx}}{\mbox{d}}x={\frac {2}{15b^{2}}}(3bx-2a)(a+bx)^{\frac {3}{2}}+C\end{equation}\begin{equation} \int x{\sqrt {a+bx}}{\mbox{d}}x={\frac {2}{15b^{2}}}(3bx-2a)(a+bx)^{\frac {3}{2}}+C\end{equation}
\begin{equation} \int x^{2}{\sqrt {a+bx}}{\mbox{d}}x={\frac {2}{105b^{3}}}(15b^{2}x^{2}-12abx+8a^{2})(a+bx)^{\frac {3}{2}}+C\end{equation}\begin{equation} \int x^{2}{\sqrt {a+bx}}{\mbox{d}}x={\frac {2}{105b^{3}}}(15b^{2}x^{2}-12abx+8a^{2})(a+bx)^{\frac {3}{2}}+C\end{equation}
\begin{equation} \int x^{n}{\sqrt {a+bx}}{\mbox{d}}x={\frac {2}{b(2n+3)}}x^{n}(a+bx)^{\frac {3}{2}}-{\frac {2na}{b(2n+3)}}\int x^{n-1}{\sqrt {a+bx}}{\mbox{d}}x\end{equation}\begin{equation} \int x^{n}{\sqrt {a+bx}}{\mbox{d}}x={\frac {2}{b(2n+3)}}x^{n}(a+bx)^{\frac {3}{2}}-{\frac {2na}{b(2n+3)}}\int x^{n-1}{\sqrt {a+bx}}{\mbox{d}}x\end{equation}
\begin{equation} \int {\frac {\sqrt {a+bx}}{x}}{\mbox{d}}x=2{\sqrt {a+bx}}+a\int {\frac {1}{x{\sqrt {a+bx}}}}{\mbox{d}}x\end{equation}\begin{equation} \int {\frac {\sqrt {a+bx}}{x}}{\mbox{d}}x=2{\sqrt {a+bx}}+a\int {\frac {1}{x{\sqrt {a+bx}}}}{\mbox{d}}x\end{equation}
\begin{equation} \int {\frac {\sqrt {a+bx}}{x^{n}}}{\mbox{d}}x={\frac {-1}{a(n-1)}}{\frac {(a+bx)^{\frac {3}{2}}}{x^{n-1}}}-{\frac {(2n-5)b}{2a(n-1)}}\int {\frac {\sqrt {a+bx}}{x^{n-1}}}{\mbox{d}}x,n\neq 1\end{equation}\begin{equation} \int {\frac {\sqrt {a+bx}}{x^{n}}}{\mbox{d}}x={\frac {-1}{a(n-1)}}{\frac {(a+bx)^{\frac {3}{2}}}{x^{n-1}}}-{\frac {(2n-5)b}{2a(n-1)}}\int {\frac {\sqrt {a+bx}}{x^{n-1}}}{\mbox{d}}x,n\neq 1\end{equation}
\begin{equation} 
\begin{aligned}
\int {\frac {1}{x{\sqrt {a+bx}}}}\mbox{d}x=&\frac {1}{\sqrt {a}}\ln \left(\frac {\sqrt {a+bx}-\sqrt {a}}{\sqrt {a+bx}+\sqrt {a}}\right)+C,a > 0 \newline
=&\frac {2}{\sqrt {-a}}\arctan {\sqrt {\frac {a+bx}{-a}}}+C,a < 0
\end{aligned}
\end{equation}
\begin{equation} 
\begin{aligned}
\int {\frac {1}{x{\sqrt {a+bx}}}}\mbox{d}x=\frac {1}{\sqrt {a}}\ln \left(\frac {\sqrt {a+bx}-\sqrt {a}}{\sqrt {a+bx}+\sqrt {a}}\right)+C,
\end{aligned}
\end{equation}
\begin{equation} \int {\frac {x}{\sqrt {a+bx}}}{\mbox{d}}x={\frac {2(a+bx)^{\frac {3}{2}}}{3b^{2}}}-{\frac {(2a){\sqrt {a+bx}}}{b^{2}}}\end{equation}\begin{equation} \int {\frac {x}{\sqrt {a+bx}}}{\mbox{d}}x={\frac {2(a+bx)^{\frac {3}{2}}}{3b^{2}}}-{\frac {(2a){\sqrt {a+bx}}}{b^{2}}}
\end{equation}
\begin{equation} \int {\frac {1}{x^{n}{\sqrt {a+bx}}}}{\mbox{d}}x={\frac {-1}{a(n-1)}}{\frac {\sqrt {a+bx}}{x^{n-1}}}-{\frac {(2n-3)b}{2a(n-1)}}\int {\frac {1}{x^{n-1}}}{\sqrt {a+bx}}{\mbox{d}}x,n\neq 1
\end{equation}
\begin{equation} \int {\frac {1}{x^{n}{\sqrt {a+bx}}}}{\mbox{d}}x={\frac {-1}{a(n-1)}}{\frac {\sqrt {a+bx}}{x^{n-1}}}-{\frac {(2n-3)b}{2a(n-1)}}\int {\frac {1}{x^{n-1}}}{\sqrt {a+bx}}{\mbox{d}}x,n\neq 1
\end{equation}
## 含有$x^2\pm\alpha^2$的积分
\begin{equation} 
\int {\frac {1}{x^{2}+\alpha ^{2}}}{\mbox{d}}x={\frac {\arctan {\dfrac {x}{\alpha }}}{\alpha }}+C
\end{equation}
\begin{equation} 
\int {\frac {1}{\pm x^{2}\mp \alpha ^{2}}}{\mbox{d}}x={\frac {\ln \left({\dfrac {x\mp \alpha }{\pm x+\alpha }}\right)}{2\alpha }}+C
\end{equation}

## 含有${ax^2+b}$的积分
 \begin{equation} 
 \int {\frac {1}{ax^{2}+b}}{\mbox{d}}x={\frac {1}{\sqrt {ab}}}\arctan {\frac {{\sqrt {a}}x}{\sqrt {b}}}+C
 \end{equation}

## 含有$ax^{2}+bx+c$的积分
 \begin{equation} \int ax^{2}+bx+c{\mbox{d}}x={\frac {ax^{3}}{3}}+{\frac {bx^{2}}{2}}+cx+C
 \end{equation}

## 含有$\sqrt{a^2+x^2}\qquad(a>0)$的积分
\begin{equation} \int {\sqrt {a^{2}+x^{2}}}{\mbox{d}}x={\frac {1}{2}}x{\sqrt {a^{2}+x^{2}}}+{\frac {1}{2}}a^{2}\ln \left(x+{\sqrt {a^{2}+x^{2}}}\right)+C\end{equation}\begin{equation} \int {\sqrt {a^{2}+x^{2}}}{\mbox{d}}x={\frac {1}{2}}x{\sqrt {a^{2}+x^{2}}}+{\frac {1}{2}}a^{2}\ln \left(x+{\sqrt {a^{2}+x^{2}}}\right)+C\end{equation}
\begin{equation} \int x^{2}{\sqrt {a^{2}+x^{2}}}{\mbox{d}}x={\frac {1}{8}}x(a^{2}+2x^{2}){\sqrt {a^{2}+x^{2}}}-{\frac {1}{8}}a^{4}\ln \left(x+{\sqrt {a^{2}+x^{2}}}\right)+C\end{equation}\begin{equation} \int x^{2}{\sqrt {a^{2}+x^{2}}}{\mbox{d}}x={\frac {1}{8}}x(a^{2}+2x^{2}){\sqrt {a^{2}+x^{2}}}-{\frac {1}{8}}a^{4}\ln \left(x+{\sqrt {a^{2}+x^{2}}}\right)+C\end{equation}
\begin{equation} \int {\frac {\sqrt {a^{2}+x^{2}}}{x}}{\mbox{d}}x={\sqrt {a^{2}+x^{2}}}-a\ln \left({\frac {a+{\sqrt {a^{2}+x^{2}}}}{x}}\right)+C\end{equation}\begin{equation} \int {\frac {\sqrt {a^{2}+x^{2}}}{x}}{\mbox{d}}x={\sqrt {a^{2}+x^{2}}}-a\ln \left({\frac {a+{\sqrt {a^{2}+x^{2}}}}{x}}\right)+C\end{equation}
\begin{equation} \int {\frac {\sqrt {a^{2}+x^{2}}}{x^{2}}}{\mbox{d}}x=\ln \left(x+{\sqrt {a^{2}+x^{2}}}\right)-{\frac {\sqrt {a^{2}+x^{2}}}{x}}+C\end{equation}\begin{equation} \int {\frac {\sqrt {a^{2}+x^{2}}}{x^{2}}}{\mbox{d}}x=\ln \left(x+{\sqrt {a^{2}+x^{2}}}\right)-{\frac {\sqrt {a^{2}+x^{2}}}{x}}+C\end{equation}
\begin{equation} \int {\frac {1}{\sqrt {a^{2}+x^{2}}}}{\mbox{d}}x=\ln \left(x+{\sqrt {a^{2}+x^{2}}}\right)+C\end{equation}\begin{equation} \int {\frac {1}{\sqrt {a^{2}+x^{2}}}}{\mbox{d}}x=\ln \left(x+{\sqrt {a^{2}+x^{2}}}\right)+C\end{equation}
\begin{equation} \int {\frac {x^{2}}{\sqrt {a^{2}+x^{2}}}}{\mbox{d}}x={\frac {1}{2}}x{\sqrt {a^{2}+x^{2}}}-{\frac {1}{2}}a^{2}\ln \left({\sqrt {a^{2}+x^{2}}}+x\right)+C\end{equation}\begin{equation} \int {\frac {x^{2}}{\sqrt {a^{2}+x^{2}}}}{\mbox{d}}x={\frac {1}{2}}x{\sqrt {a^{2}+x^{2}}}-{\frac {1}{2}}a^{2}\ln \left({\sqrt {a^{2}+x^{2}}}+x\right)+C\end{equation}
\begin{equation} \int {\frac {1}{x{\sqrt {a^{2}+x^{2}}}}}{\mbox{d}}x={\frac {1}{a}}\ln \left({\frac {x}{a+{\sqrt {a^{2}+x^{2}}}}}\right)+C\end{equation}\begin{equation} \int {\frac {1}{x{\sqrt {a^{2}+x^{2}}}}}{\mbox{d}}x={\frac {1}{a}}\ln \left({\frac {x}{a+{\sqrt {a^{2}+x^{2}}}}}\right)+C\end{equation}
\begin{equation} \int {\frac {1}{x^{2}{\sqrt {a^{2}+x^{2}}}}}{\mbox{d}}x=-{\frac {\sqrt {a^{2}+x^{2}}}{a^{2}x}}+C\end{equation}\begin{equation} \int {\frac {1}{x^{2}{\sqrt {a^{2}+x^{2}}}}}{\mbox{d}}x=-{\frac {\sqrt {a^{2}+x^{2}}}{a^{2}x}}+C
\end{equation}

## 含有$\sqrt{x^2-a^2}\qquad{(x^2>a^2)}$的积分
\begin{equation} \int {\frac {1}{\sqrt {x^{2}-a^{2}}}}{\mbox{d}}x=\ln \vert x+{\sqrt {x^{2}-a^{2}}}\vert +C
\end{equation}

## 含有$\sqrt{a^2-x^2} \qquad(a^2>x^2)$的积分
\begin{equation} \int {\sqrt {a^{2}-x^{2}}}{\mbox{d}}x={\frac {1}{2}}x{\sqrt {a^{2}-x^{2}}}+{\frac {a^{2}}{2}}\arcsin {\frac {x}{a}}+C\end{equation}\begin{equation} \int {\sqrt {a^{2}-x^{2}}}{\mbox{d}}x={\frac {1}{2}}x{\sqrt {a^{2}-x^{2}}}+{\frac {a^{2}}{2}}\arcsin {\frac {x}{a}}+C\end{equation}
\begin{equation} \int {\frac {1}{\sqrt {a^{2}-x^{2}}}}{\mbox{d}}x=\arcsin {\frac {x}{a}}+C=-\arccos {\frac {x}{a}}+C\end{equation}\begin{equation} \int {\frac {1}{\sqrt {a^{2}-x^{2}}}}{\mbox{d}}x=\arcsin {\frac {x}{a}}+C=-\arccos {\frac {x}{a}}+C\end{equation}
\begin{equation} \int x^{2}{\sqrt {a^{2}-x^{2}}}{\mbox{d}}x={\frac {1}{8}}x(2x^{2}-a^{2}){\sqrt {a^{2}-x^{2}}}+{\frac {1}{8}}a^{4}\arcsin {\frac {x}{a}}+C\end{equation}\begin{equation} \int x^{2}{\sqrt {a^{2}-x^{2}}}{\mbox{d}}x={\frac {1}{8}}x(2x^{2}-a^{2}){\sqrt {a^{2}-x^{2}}}+{\frac {1}{8}}a^{4}\arcsin {\frac {x}{a}}+C\end{equation}
\begin{equation} \int {\frac {\sqrt {a^{2}-x^{2}}}{x}}{\mbox{d}}x={\sqrt {a^{2}-x^{2}}}-a\ln \left({\frac {a+{\sqrt {a^{2}-x^{2}}}}{x}}\right)+C\end{equation}\begin{equation} \int {\frac {\sqrt {a^{2}-x^{2}}}{x}}{\mbox{d}}x={\sqrt {a^{2}-x^{2}}}-a\ln \left({\frac {a+{\sqrt {a^{2}-x^{2}}}}{x}}\right)+C\end{equation}
\begin{equation} \int {\frac {\sqrt {a^{2}-x^{2}}}{x^{2}}}{\mbox{d}}x=-{\frac {\sqrt {a^{2}-x^{2}}}{x}}-\arcsin {\frac {x}{a}}+C\end{equation}\begin{equation} \int {\frac {\sqrt {a^{2}-x^{2}}}{x^{2}}}{\mbox{d}}x=-{\frac {\sqrt {a^{2}-x^{2}}}{x}}-\arcsin {\frac {x}{a}}+C\end{equation}
\begin{equation} \int {\frac {1}{x{\sqrt {a^{2}-x^{2}}}}}{\mbox{d}}x=-{\frac {1}{a}}\ln \left({\frac {a+{\sqrt {a^{2}-x^{2}}}}{x}}\right)+C\end{equation}\begin{equation} \int {\frac {1}{x{\sqrt {a^{2}-x^{2}}}}}{\mbox{d}}x=-{\frac {1}{a}}\ln \left({\frac {a+{\sqrt {a^{2}-x^{2}}}}{x}}\right)+C\end{equation}
\begin{equation} \int {\frac {x^{2}}{\sqrt {a^{2}-x^{2}}}}{\mbox{d}}x=-{\frac {1}{2}}x{\sqrt {a^{2}-x^{2}}}+{\frac {1}{2}}a^{2}\arcsin {\frac {x}{a}}+C\end{equation}\begin{equation} \int {\frac {x^{2}}{\sqrt {a^{2}-x^{2}}}}{\mbox{d}}x=-{\frac {1}{2}}x{\sqrt {a^{2}-x^{2}}}+{\frac {1}{2}}a^{2}\arcsin {\frac {x}{a}}+C\end{equation}
\begin{equation} \int {\frac {1}{x^{2}{\sqrt {a^{2}-x^{2}}}}}{\mbox{d}}x=-{\frac {\sqrt {a^{2}-x^{2}}}{a^{2}x}}+C\end{equation}\begin{equation} \int {\frac {1}{x^{2}{\sqrt {a^{2}-x^{2}}}}}{\mbox{d}}x=-{\frac {\sqrt {a^{2}-x^{2}}}{a^{2}x}}+C
\end{equation}

## 含有$R=\sqrt{\vert a\vert x^2+bx+c}\qquad(a\ne0)$的积分
\begin{equation} 
\int {\frac {{\mbox{d}}x}{R}}={\frac {1}{\sqrt {a}}}\ln \left(2{\sqrt {a}}R+2ax+b\right)\qquad ({\mbox{for }}a > 0)
\end{equation}
\begin{equation} 
\int {\frac {{\mbox{d}}x}{R}}={\frac {1}{\sqrt {a}}}\,\operatorname {arsinh} {\frac {2ax+b}{\sqrt {4ac-b^{2}}}}\qquad {\mbox{(for }}a > 0{\mbox{, }}4ac-b^{2} > 0{\mbox{)}}
\end{equation}
\begin{equation} 
\int {\frac {{\mbox{d}}x}{R}}={\frac {1}{\sqrt {a}}}\ln \vert 2ax+b\vert \quad {\mbox{(for }}a > 0{\mbox{, }}4ac-b^{2}=0{\mbox{)}}
\end{equation}
\begin{equation} 
\int {\frac {{\mbox{d}}x}{R}}=-{\frac {1}{\sqrt {-a}}}\arcsin {\frac {2ax+b}{\sqrt {b^{2}-4ac}}}\qquad {\mbox{(for }}a<0{\mbox{, }}4ac-b^{2} < 0{\mbox{, }}\left(2ax+b\right)<{\sqrt {b^{2}-4ac}}{\mbox{)}}\end{equation}
\begin{equation} 
\int {\frac {{\mbox{d}}x}{R^{3}}}={\frac {4ax+2b}{(4ac-b^{2})R}}\end{equation}
\begin{equation} 
\int {\frac {{\mbox{d}}x}{R^{5}}}={\frac {4ax+2b}{3(4ac-b^{2})R}}\left({\frac {1}{R^{2}}}+{\frac {8a}{4ac-b^{2}}}\right)\end{equation}
\begin{equation} 
\int {\frac {{\mbox{d}}x}{R^{2n+1}}}={\frac {2}{(2n-1)(4ac-b^{2})}}\left[{\frac {2ax+b}{R^{2n-1}}}+4a(n-1)\int {\frac {{\mbox{d}}x}{R^{2n-1}}}\right]\end{equation}
\begin{equation} 
\int {\frac {x}{R}}\;{\mbox{d}}x={\frac {R}{a}}-{\frac {b}{2a}}\int {\frac {{\mbox{d}}x}{R}}
\end{equation}
\begin{equation} 
\int {\frac {x}{R^{3}}}\;{\mbox{d}}x=-{\frac {2bx+4c}{(4ac-b^{2})R}}
\end{equation}
\begin{equation} \int {\frac {x}{R^{2n+1}}}\;{\mbox{d}}x=-{\frac {1}{(2n-1)aR^{2n-1}}}-{\frac {b}{2a}}\int {\frac {{\mbox{d}}x}{R^{2n+1}}}\end{equation}
\begin{equation} \int {\frac {{\mbox{d}}x}{xR}}=-{\frac {1}{\sqrt {c}}}\ln \left({\frac {2{\sqrt {c}}R+bx+2c}{x}}\right)\end{equation}
\begin{equation} \int {\frac {{\mbox{d}}x}{xR}}=-{\frac {1}{\sqrt {c}}}\operatorname {arsinh} \left({\frac {bx+2c}{\vert x\vert {\sqrt {4ac-b^{2}}}}}\right)\end{equation}


## 含有三角函数的积分
\begin{equation} 
\int \cos x{\mbox{d}}x=\sin x+C
\end{equation}
\begin{equation} 
\int \sin x{\mbox{d}}x=-\cos x+C
\end{equation}
\begin{equation} 
\int \sec ^{2}x{\mbox{d}}x=\tan x+C
\end{equation}
\begin{equation} 
\int \csc ^{2}x{\mbox{d}}x=-\cot x+C
\end{equation}
\begin{equation} 
\int \sec x\tan x{\mbox{d}}x=\sec x+C
\end{equation}
\begin{equation} 
\int \csc x\cot x{\mbox{d}}x=-\csc x+C
\end{equation}
\begin{equation} 
\int \tan x{\mbox{d}}x=-\ln {\left\vert \cos {x}\right\vert}+C=\ln {\left\vert \sec x\right\vert}+C
\end{equation}
\begin{equation} 
\int \cot x{\mbox{d}}x=\ln {\left\vert \sin x\right\vert}+C
\end{equation}
\begin{equation} 
\int \sec x{\mbox{d}}x=\ln {\left\vert \sec x+\tan x\right\vert}+C
\end{equation}
\begin{equation} 
\int \csc x{\mbox{d}}x=\ln {\left\vert \csc x-\cot x\right\vert}+C=\ln {\left\vert {\tan x-\sin x \over \sin x\tan x}\right\vert}+C
\end{equation}
\begin{equation} 
\int \sin ^{n}x{\mbox{d}}x=-{\frac {1}{n}}\sin ^{n-1}x\cos x+{\frac {n-1}{n}}\int \sin ^{n-2}x{\mbox{d}}x+C\quad \forall n\geq 2
\end{equation}
\begin{equation} 
\int \sin ^{2}x{\mbox{d}}x={\frac {x}{2}}-{\frac {\sin {2x}}{4}}+C
\end{equation}
\begin{equation} 
\int \cos ^{n}x{\mbox{d}}x={\frac {1}{n}}\cos ^{n-1}x\sin x+{\frac {n-1}{n}}\int \cos ^{n-2}x{\mbox{d}}x+C\quad \forall n\geq 2
\end{equation}
\begin{equation} 
\int \cos ^{2}x{\mbox{d}}x={\frac {x}{2}}+{\frac {\sin {2x}}{4}}+C
\end{equation}
\begin{equation} 
\int \tan ^{n}x{\mbox{d}}x={\frac {1}{n-1}}\tan ^{n-1}x-\int \tan ^{n-2}x{\mbox{d}}x+C\quad \forall n\geq 2\end{equation}
\begin{equation} \int \tan ^{2}x{\mbox{d}}x=\tan x-x+C\end{equation}
\begin{equation} \int \cot ^{n}x{\mbox{d}}x={\frac {1}{n-1}}\cot ^{n-1}x-\int \cot ^{n-2}x{\mbox{d}}x+C\quad \forall n\geq 2\end{equation}
\begin{equation} \int \cot ^{2}x{\mbox{d}}x=-\cot x-x+C\end{equation}
\begin{equation} \int \sec ^{n}x{\mbox{d}}x={\frac {1}{n-1}}\sec ^{n-2}x\tan x+{\frac {n-2}{n-1}}\int \sec ^{n-2}x{\mbox{d}}x+C\quad \forall n\geq 2
\end{equation}
\begin{equation} 
\int \csc ^{n}x{\mbox{d}}x=-{\frac {1}{n-1}}\csc ^{n-2}x\cot x+{\frac {n-2}{n-1}}\int \csc ^{n-2}x{\mbox{d}}x+C\quad \forall n\geq 2
\end{equation}


## 含有反三角函数的积分
\begin{equation} \int \arcsin x{\mbox{d}}x=x\arcsin x+{\sqrt {1-x^{2}}}+C\end{equation}\begin{equation} \int \arcsin x{\mbox{d}}x=x\arcsin x+{\sqrt {1-x^{2}}}+C\end{equation}
\begin{equation} \int \arccos x{\mbox{d}}x=x\arccos x-{\sqrt {1-x^{2}}}+C\end{equation}\begin{equation} \int \arccos x{\mbox{d}}x=x\arccos x-{\sqrt {1-x^{2}}}+C\end{equation}
\begin{equation} \int \arctan {x}\,dx=x\arctan {x}-{\frac {1}{2}}\ln {\vert 1+x^{2}\vert }+C\end{equation}\begin{equation} \int \arctan {x}\,dx=x\arctan {x}-{\frac {1}{2}}\ln {\vert 1+x^{2}\vert }+C\end{equation}
\begin{equation} \int \operatorname {arccot} {x}\,dx=x\operatorname {arccot} {x}+{\frac {1}{2}}\ln {\vert 1+x^{2}\vert }+C\end{equation}\begin{equation} \int \operatorname {arccot} {x}\,dx=x\operatorname {arccot} {x}+{\frac {1}{2}}\ln {\vert 1+x^{2}\vert }+C\end{equation}
\begin{equation} \int \operatorname {arcsec} x{\mbox{d}}x=x\operatorname {arcsec} x-\operatorname {sgn} (x)\ln \left\vert x+{\sqrt {x^{2}-1}}\right\vert+C=x\operatorname {arcsec} x+\operatorname {sgn} (x)\ln \left\vert x-{\sqrt {x^{2}-1}}\right\vert+C\end{equation}\begin{equation} \int \operatorname {arcsec} x{\mbox{d}}x=x\operatorname {arcsec} x-\operatorname {sgn}(x)\ln \left\vert x+{\sqrt {x^{2}-1}}\right\vert+C=x\operatorname {arcsec} x+\operatorname {sgn}(x)\ln \left\vert x-{\sqrt {x^{2}-1}}\right\vert+C\end{equation}
\begin{equation} \int \operatorname {arccsc} x{\mbox{d}}x=x\operatorname {arccsc} x+\operatorname {sgn}(x)\ln \left\vert x+{\sqrt {x^{2}-1}}\right\vert+C=x\operatorname {arccsc} x-\operatorname {sgn}(x)\ln \left\vert x-{\sqrt {x^{2}-1}}\right\vert+C\end{equation}\begin{equation} \int \operatorname {arccsc} x{\mbox{d}}x=x\operatorname {arccsc} x+\operatorname {sgn}(x)\ln \left\vert x+{\sqrt {x^{2}-1}}\right\vert+C=x\operatorname {arccsc} x-\operatorname {sgn}(x)\ln \left\vert x-{\sqrt {x^{2}-1}}\right\vert+C
\end{equation}

## 含有指数函数的积分
\begin{equation} \int e^{x}{\mbox{d}}x=e^{x}+C
\end{equation}
\begin{equation} \int \alpha ^{x}{\mbox{d}}x={\frac {\alpha ^{x}}{\ln \alpha }}+C
\end{equation}
\begin{equation} \int xe^{ax}{\mbox{d}}x={\frac {1}{a^{2}}}(ax-1)e^{ax}+C
\end{equation}
\begin{equation} \int x^{n}e^{ax}{\mbox{d}}x={\frac {1}{a}}x^{n}e^{ax}-{\frac {n}{a}}\int x^{n-1}e^{ax}{\mbox{d}}x
\end{equation}
\begin{equation} \int e^{ax}\sin bx{\mbox{d}}x={\frac {e^{ax}}{a^{2}+b^{2}}}(a\sin bx-b\cos bx)+C
\end{equation}
\begin{equation} \int e^{ax}\cos bx{\mbox{d}}x={\frac {e^{ax}}{a^{2}+b^{2}}}(a\cos bx+b\sin bx)+C
\end{equation}

## 含有对数函数的积分
\begin{equation} \int \ln x{\mbox{d}}x=x\ln x-x+C
\end{equation}
\begin{equation} \int \log _ {\alpha }x{\mbox{d}}x={\frac {1}{\ln \alpha }}\left({x\ln x-x}\right)+C
\end{equation}
\begin{equation} \int x^{n}\ln x{\mbox{d}}x={\frac {x^{n+1}}{(n+1)^{2}}}[(n+1)\ln x-1]+C
\end{equation}
\begin{equation} \int {\frac {1}{x\ln {x}}}{\mbox{d}}x=\ln {(\ln {x})}+C
\end{equation}

## 含有双曲函数的积分
\begin{equation} \int \sinh x{\mbox{d}}x=\cosh x+C
\end{equation}
\begin{equation} \int \cosh x{\mbox{d}}x=\sinh x+C
\end{equation}
\begin{equation} \int \tanh x{\mbox{d}}x=\ln \left(\cosh x\right)+C
\end{equation}
\begin{equation} \int \coth x{\mbox{d}}x=\ln \left\vert \sinh x\right\vert+C
\end{equation}
\begin{equation} \int {\mbox{sech}}\ x{\mbox{d}}x=\arcsin \left(\tanh x\right)+C=\arctan \left(\sinh x\right)+C
\end{equation}
\begin{equation} \int {\mbox{csch}}\ x{\mbox{d}}x=\ln \left\vert \tanh {x \over 2}\right\vert+C
\end{equation}

## 定积分
\begin{equation} \int_{-\infty }^{\infty }e^{-\alpha x^{2}}{\mbox{d}}x={\sqrt {\frac {\pi }{\alpha }}}
\end{equation}
\begin{equation} 
\int_{0}^{\frac {\pi }{2}}{\mbox{sin}}^{n}x{\mbox{d}}x=\int _{0}^{\frac {\pi }{2}}{\mbox{cos}}^{n}x{\mbox{d}}x={\begin{cases}{\frac {n-1}{n}}\cdot {\frac {n-3}{n-2}}\cdot \ldots \cdot {\frac {4}{5}}\cdot {\frac {2}{3}},&{\mbox{if }}n>1{\mbox{ 且 }}n{\mbox{为 奇 数 }}\newline
{\frac {n-1}{n}}\cdot {\frac {n-3}{n-2}}\cdot \ldots \cdot {\frac {3}{4}}\cdot {\frac {1}{2}}\cdot {\frac {\pi }{2}},&{\mbox{if }}n>0{\mbox{ 且 }}n{\mbox{为 偶 数 }}
\end{cases}}
\end{equation}