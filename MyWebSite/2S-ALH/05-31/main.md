
<!-- > pandoc main.md --mathjax -c ../../css/mathjax.css --include-in-header=../in-header.txt --include-before-body=../before-body.txt --include-after-body=../after-body.txt -s -o main.html -->

**2S-ALH @2017/05/31 “いろいろな関数の導関数”**

# 合成関数の導関数

$\frac{dy}{dx}=\frac{dy}{du}\frac{du}{dx}=f'(u)g'(x)=f'(g(x))g'(x)$

### 問題A. $y=(3x^2-2)^6$ を微分せよ．

>　  
>　

### 問題B. $y=(9-x^3)^3$ を微分せよ．

>　  
>　

### 問題C. $y=\cos^3 x$ を微分せよ．

>　  
>　

### 問題D. $y=\tan^2(3x-4)$ を微分せよ．

>　  
>　  
>　

<div style="page-break-before:always"></div>

### 問題E. $y=\sqrt[4]{x^3+6x-7}$ を微分せよ．

>　  
>　  
> 　

# 対数関数の導関数

$\{f^{-1}(x)\}'=\frac{1}{f'(y)}$ ただし $f'(y)\ne0$

### 問題A. $y=x^2\log x$ を微分せよ．

>　  
>　

### 問題B. $y=\frac{x+1}{\log x}$ を微分せよ．

>　  
>　

### 問題C. $y=\log\frac{x^2}{\cos x}$ を微分せよ．

>　  
>　

## 対数微分法

両辺の対数をとって微分する．

### 問題A. $y=x^\pi$ を微分せよ．

>　  
>　  
>　  
>　

### 問題B. $y=\frac{1}{x^e}$ を微分せよ．

>　  
>　  
>　  
>　  
>　

### 問題C. $y=x^{2x}$ を微分せよ．ただし $x>0$ とする．

>　  
>　  
>　  
>　

<div style="page-break-before:always"></div>

## 絶対値の微分

正の場合と負の場合に分けて考える．

### 問題A. $y=\log|x^2-1|$ を微分せよ．

>　  
>　  
>　  
>　  
>　

### 問題B. $y=\log|e^x-2|$ を微分せよ．

>　  
>　  
>　  
>　  
>　

<div style="page-break-before:always"></div>

## 逆三角関数とその導関数

- $(\sin^{-1} x)'=\frac{1}{\sqrt{1-x^2}}$
- $(\cos^{-1} x)'=-\frac{1}{\sqrt{1-x^2}}$
- $(\tan^{-1} x)'=\frac{1}{1+x^2}$

### 問題A. $y=\sin^{-1} 3x$ を微分せよ．

>　  
>　

### 問題B. $y=\cos^{-1} x^2$ を微分せよ．

>　  
>　

### 問題C. $y=\tan^{-1} (-\sqrt{x})$ を微分せよ．

>　  
>　

<div style="page-break-before:always"></div>

### 問題D. $y=\sqrt{\tan^{-1} x}$ を微分せよ．

>　  
>　  

<div style="page-break-before:always"></div>

## 関数の連続 - 中間値の定理

関数 $f(x)$ が閉区間 $[a,b]$ で連続で，$f(a)\ne f(b)$ のとき，$f(a)$ と $f(b)$ の間にある任意の値 $k$ に対して  
　$f(c)=k (a<c<b)$  
を満たす点 $c$ が少なくとも1つ存在する．

### 問題. 上記は関数が連続でなければ成り立たない．そのような例（中間値をもたない例）を挙げよ．

>　  
> 　

## 連続関数の最大値と最小値

閉区間 $[a,b]$ で連続な関数 $f(x)$ は，この区間で必ず最大値と最小値をもつ．

### 問題. 上記は開区間に対しては成り立たない．そのような例（連続だが最大値あるいは最小値をもたない例）を挙げよ．

>　  
> 　

<div style="page-break-before:always"></div>

---

この資料と解答はwebで公開しています：  
![](../QRcode.png)  
**情報工学科のサイト（「大分高専 情報」で検索）→ スタッフ紹介（教職員紹介） → 西村俊二 → 一番下のリンク → 2S ALH**

---

解説及び問題は下記より：  
　高遠節夫他，「新微分積分I問題集」，大日本図書
