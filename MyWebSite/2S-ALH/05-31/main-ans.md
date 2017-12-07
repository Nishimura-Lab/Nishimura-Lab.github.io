
<!-- > pandoc main-ans.md --mathjax -c ../../css/mathjax.css --include-in-header=../in-header.txt --include-before-body=../before-body.txt --include-after-body=../after-body.txt -s -o main-ans.html -->

**2S-ALH @2017/05/31 “いろいろな関数の導関数”**

# 合成関数の導関数

$\frac{dy}{dx}=\frac{dy}{du}\frac{du}{dx}=f'(u)g'(x)=f'(g(x))g'(x)$

### 問題A. $y=(3x^2-2)^6$ を微分せよ．

> $y'=6(3x^2-2)^5\cdot3\cdot2x$  
> $=36x(3x^2-2)^5$

### 問題B. $y=(9-x^3)^3$ を微分せよ．

> $y'=3(9-x^3)^2\cdot(-3x^2)$  
> $=-9x^2(9-x^3)^2$

### 問題C. $y=\cos^3 x$ を微分せよ．

> $y'=3\cos^2x\cdot(-\sin x)$  
> $=-3\cos^2x\sin x$

### 問題D. $y=\tan^2(3x-4)$ を微分せよ．

> $y'=2\tan(3x-4)\cdot(\tan(3x-4))'$  
> $=2\tan(3x-4)\cdot\frac{1}{\cos^2(3x-4)}\cdot3$  
> $=\frac{6\tan(3x-4)}{\cos^2(3x-4)}$

<div style="page-break-before:always"></div>

### 問題E. $y=\sqrt[4]{x^3+6x-7}$ を微分せよ．

> $y'=\frac{1}{4}\cdot\frac{1}{\sqrt[4]{(x^3+6x-7)^3}\cdot(3x^2+6)}$  
> $=\frac{3x^2+6}{4\sqrt[4]{(x^2+6x-7)^3}}$  
> 　

# 対数関数の導関数

$\{f^{-1}(x)\}'=\frac{1}{f'(y)}$ ただし $f'(y)\ne0$

### 問題A. $y=x^2\log x$ を微分せよ．

> $y'=2x\log x+x^2\cdot\frac{1}{x}$  
> $= 2x\log x+x$

### 問題B. $y=\frac{x+1}{\log x}$ を微分せよ．

> $y'=\frac{1\cdot\log x-(x+1)\cdot\frac{1}{x}}{\log^2 x}$  
> $=\frac{\log x-1-\frac{1}{x}}{\log^2 x}$ $=\frac{x\log x-x-1}{x\log^2 x}$

### 問題C. $y=\log\frac{x^2}{\cos x}$ を微分せよ．

> $y'=\frac{1}{\frac{x^2}{\cos x}}\cdot\frac{2x\cos x-x^2\cdot(-\sin x)}{\cos^2 x}$  
> $=\frac{2\cos x+x\sin x}{x\cos x}$ $=\frac{2}{x}+\tan x$

## 対数微分法

両辺の対数をとって微分する．

### 問題A. $y=x^\pi$ を微分せよ．

> $\log y=\pi\log x$ を微分すると，  
> $\frac{d}{dx}(\log y)=\frac{d}{dx}(\pi\log x)$  
> $\frac{d}{dy}(\log y)\cdot\frac{dy}{dx}=\pi\cdot\frac{1}{x}$  
> $\frac{1}{y}\cdot y'=\frac{\pi}{x}$ ∴ $y'=\frac{\pi y}{x}$ $=\frac{\pi x^\pi}{x}$ $=\pi x^{\pi-1}$

### 問題B. $y=\frac{1}{x^e}$ を微分せよ．

> $\log y=\log x^{-e}$ を微分すると，  
> $\frac{d}{dx}(\log y)=\frac{d}{dx}(\log x^{-e})$  
> $\frac{d}{dy}(\log y)\cdot\frac{dy}{dx}=\frac{d}{dy}(\log x^{-e})\cdot\frac{dy}{dx}$  
> $\frac{1}{y}\cdot y'=\frac{1}{x^{-e}}(-e)x^{(-e-1)}$  
> ∴ $y'=\frac{y}{x^{-e}}(-e)x^{-(e+1)}$ $=\frac{x^{-e}}{x^{-e}}(-\frac{e}{x^{e+1}})$ $=-\frac{e}{x^{e+1}}$

### 問題C. $y=x^{2x}$ を微分せよ．ただし $x>0$ とする．

> $\log y=\log x^{2x}=2x\log x$  
> $\frac{1}{y}y'=2\log x+2x\frac{1}{x}$  
> 　$=2(\log x+1)$  
> ∴ $y'=2y(\log x+1)$ $=2x^{2x}(\log x+1)$

<div style="page-break-before:always"></div>

## 絶対値の微分

正の場合と負の場合に分けて考える．

### 問題A. $y=\log|x^2-1|$ を微分せよ．

> $x^2-1>0$ ⇒ $y=\log (x^2-1)$．よって  
> 　$y'=\frac{1}{x^2-1}\cdot 2x$ $=\frac{2x}{x^2-1}$  
> $x^2-1<0$ ⇒ $y=\log (-x^2+1)$．よって  
> 　$y'=\frac{1}{-x^2+1}\cdot (-2x)$ $=\frac{2x}{x^2-1}$  
> ∴ $y'=\frac{2x}{x^2-1}$

### 問題B. $y=\log|e^x-2|$ を微分せよ．

> $e^x-2>0$ ⇒ $y=\log (e^x-2)$．よって  
> 　$y'=\frac{1}{e^x-2}\cdot e^x$  
> $e^x-2<0$ ⇒ $y=\log (-e^x+2)$．よって  
> 　$y'=\frac{1}{-e^x+2}\cdot (-e^x)$  
> ∴ $y'=\frac{e^x}{e^x-2}$

<div style="page-break-before:always"></div>

## 逆三角関数とその導関数

- $(\sin^{-1} x)'=\frac{1}{\sqrt{1-x^2}}$
- $(\cos^{-1} x)'=-\frac{1}{\sqrt{1-x^2}}$
- $(\tan^{-1} x)'=\frac{1}{1+x^2}$

### 問題A. $y=\sin^{-1} 3x$ を微分せよ．

> $y'=\frac{1}{\sqrt{1-9x^2}}\cdot 3$  
> $=\frac{3}{\sqrt{1-9x^2}}$

### 問題B. $y=\cos^{-1} x^2$ を微分せよ．

> $y'=-\frac{1}{\sqrt{1-x^4}}\cdot 2x$  
> $=-\frac{2x}{\sqrt{1-x^4}}$

### 問題C. $y=\tan^{-1} (-\sqrt{x})$ を微分せよ．

> $y'=\frac{1}{1+(-\sqrt{x})^2}\cdot(-\frac{1}{2})\cdot\frac{1}{\sqrt{x}}$  
> $=-\frac{1}{2\sqrt{x}(x+1)}$

<div style="page-break-before:always"></div>

### 問題D. $y=\sqrt{\tan^{-1} x}$ を微分せよ．

> $y'=\frac{1}{2}(\tan^{-1} x)^{-\frac{1}{2}}\cdot\frac{1}{1+x^2}$  
> $=\frac{1}{2(x^2+1)\sqrt{\tan^{-1} x}}$  

<div style="page-break-before:always"></div>

## 関数の連続 - 中間値の定理

関数 $f(x)$ が閉区間 $[a,b]$ で連続で，$f(a)\ne f(b)$ のとき，$f(a)$ と $f(b)$ の間にある任意の値 $k$ に対して  
　$f(c)=k (a<c<b)$  
を満たす点 $c$ が少なくとも1つ存在する．

### 問題. 上記は関数が連続でなければ成り立たない．そのような例（中間値をもたない例）を挙げよ．

> $x\le 0$ で $f(x)=0$，$x>0$ で $f(x)=2$ と定義された関数は $f(c)=1$ となる点 $c$ が存在しない．  
> 　

## 連続関数の最大値と最小値

閉区間 $[a,b]$ で連続な関数 $f(x)$ は，この区間で必ず最大値と最小値をもつ．

### 問題. 上記は開区間に対しては成り立たない．そのような例（連続だが最大値あるいは最小値をもたない例）を挙げよ．

> $f(x)=\frac{1}{x}$ を開区間 $(0,1]$ で考えると，これは最大値をもたない．  
> 　

<div style="page-break-before:always"></div>

---

この資料と解答はwebで公開しています：  
![](../QRcode.png)  
**情報工学科のサイト（「大分高専 情報」で検索）→ スタッフ紹介（教職員紹介） → 西村俊二 → 一番下のリンク → 2S ALH**

---

解説及び問題は下記より：  
　高遠節夫他，「新微分積分I問題集」，大日本図書
