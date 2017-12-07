
<!-- > pandoc main.md --mathjax -c ../../css/mathjax.css --include-in-header=../in-header.txt --include-before-body=../before-body.txt --include-after-body=../after-body.txt -s -o main.html -->

2017/05/24 2S ALH

# 関数の極限と導関数

## 極限値の性質

$\lim\limits_{x\rightarrow a} \{f(x)\pm g(x)\}=\lim\limits_{x\rightarrow a} f(x)\pm \lim\limits_{x\rightarrow a} g(x)$  
$\lim\limits_{x\rightarrow a} cf(x)=c\lim\limits_{x\rightarrow a} f(x)$  
$\lim\limits_{x\rightarrow a} \{f(x)g(x)\}=\lim\limits_{x\rightarrow a} f(x)\lim\limits_{x\rightarrow a} g(x)$  
$\lim\limits_{x\rightarrow a} \frac{f(x)}{g(x)}=\frac{\lim\limits_{x\rightarrow a} f(x)}{\lim\limits_{x\rightarrow a} g(x)}$  

### 問題A. $\lim\limits_{x\rightarrow 2} x^4$ の極限値を求めよ．

> 　  
> 　  
> 　  

### 問題B. $\lim\limits_{x\rightarrow 2} (x^2+2x-3)$ の極限値を求めよ．

> 　  
> 　  
> 　  

<div style="page-break-before:always"></div>

### 問題C. $\lim\limits_{x\rightarrow 0} \frac{x^3+2x}{3x}$ の極限値を求めよ．

> 　  
> 　  
> 　  

　  
　  

## 三角関数・指数関数の極限値

$\lim\limits_{\theta\rightarrow 0} \frac{\sin \theta}{\theta}=1$  
$\lim\limits_{h\rightarrow 0} \frac{e^h-1}{h}=1$  
$\lim\limits_{t\rightarrow 0} (1+t)^\frac{1}{t}$
$=\lim\limits_{x\rightarrow \pm\infty} (1+\frac{1}{x})^x=e$ 

### 問題A. $\lim\limits_{\theta\rightarrow 0} \frac{\sin \pi\theta}{\theta}$ の極限値を求めよ．

> 　  
> 　  
> 　  

<div style="page-break-before:always"></div>

### 問題B. $\lim\limits_{\theta\rightarrow 0} \frac{\theta}{\tan 3\theta}$ の極限値を求めよ．

> 　  
> 　  
> 　  

### 問題C. $\lim\limits_{\theta\rightarrow 0} \frac{\theta\sin 3\theta}{1-\cos 3\theta}$ の極限値を求めよ．

> 　  
> 　  
> 　  

<div style="page-break-before:always"></div>

## 微分係数（変化率）

$f'(a)=\lim\limits_{x\rightarrow a} \frac{f(x)-f(a)}{x-a}$ $=\lim\limits_{h\rightarrow 0} \frac{f(a+h)-f(a)}{h}$

### 問題A. $f(x)=x^3$ の $x=1$ における微分係数を求めよ．

> 　  
> 　  
> 　  

### 問題B. $f(x)=\sqrt{x}$ の $x=4$ における微分係数を求めよ．

> 　  
> 　  
> 　  

### 問題C. $f(x)=x^2-x$ の $x=1$ における微分係数を求めよ．

> 　  
> 　  
> 　  

## 導関数

$f'(x)=\lim\limits_{X\rightarrow a} \frac{f(X)-f(x)}{X-x}$ $=\lim\limits_{h\rightarrow 0} \frac{f(x+h)-f(x)}{h}$

### 問題A. $y=x^2-x$ の導関数を求めよ．

> 　  
> 　  
> 　  

### 問題B. $y=x^3+2$ の導関数を求めよ．

> 　  
> 　  
> 　  

<div style="page-break-before:always"></div>

## 導関数の性質

$(c)'=0$，$(cf)'=cf'$，$(f\pm g)'=f'\pm g'$  
$(fg)'=f'g+fg'$  
$(\frac{f}{g})'=\frac{f'g-fg'}{g^2}$  
$\{f(ax+b)\}'=af'(ax+b)$

（よく使う公式： $(x^r)'=rx^{r-1}$）

### 問題A. $y=x^4-2x^3+x$ を微分せよ．

> 　  
> 　  

### 問題B. $y=\frac{2}{3}x^3+\frac{1}{2}x-1$ を微分せよ．

> 　  
> 　  

### 問題C. $y=(x+1)(x^2-x+1)$ を微分せよ．

> 　  
> 　  

<div style="page-break-before:always"></div>

## 導関数の公式

$(x^r)'=rx^{r-1}$  
$(\sin x)'=\cos x$，$(\cos x)'=-\sin x$，$(\tan x)'=\frac{1}{\cos^2 x}$  
$(e^x)'=e^x$，$(a^x)'=a^x\log a$

### 問題A. $y=\sin(2-3x)$ を微分せよ．

> 　  
> 　  
> 　  

### 問題B. $y=\tan(x-2)$ を微分せよ．

> 　  
> 　  
> 　  

### 問題C. $y=e^{2x+5}$ を微分せよ．

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
