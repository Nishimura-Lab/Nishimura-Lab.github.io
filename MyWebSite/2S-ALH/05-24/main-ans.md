
<!-- > pandoc main-ans.md --mathjax -c ../../css/mathjax.css --include-in-header=../in-header.txt --include-before-body=../before-body.txt --include-after-body=../after-body.txt -s -o main-ans.html -->

2017/05/24 2S ALH

# 関数の極限と導関数

## 極限値の性質

$\lim\limits_{x\rightarrow a} \{f(x)\pm g(x)\}=\lim\limits_{x\rightarrow a} f(x)\pm \lim\limits_{x\rightarrow a} g(x)$  
$\lim\limits_{x\rightarrow a} cf(x)=c\lim\limits_{x\rightarrow a} f(x)$  
$\lim\limits_{x\rightarrow a} \{f(x)g(x)\}=\lim\limits_{x\rightarrow a} f(x)\lim\limits_{x\rightarrow a} g(x)$  
$\lim\limits_{x\rightarrow a} \frac{f(x)}{g(x)}=\frac{\lim\limits_{x\rightarrow a} f(x)}{\lim\limits_{x\rightarrow a} g(x)}$  

### 問題A. $\lim\limits_{x\rightarrow 2} x^4$ の極限値を求めよ．

> $=\lim\limits_{x\rightarrow 2} x\cdot x\cdot x\cdot x$  
> $=\lim\limits_{x\rightarrow 2} x\cdot\lim\limits_{x\rightarrow 2} x\cdot\lim\limits_{x\rightarrow 2} x\cdot\lim\limits_{x\rightarrow 2} x$  
> $=(\lim\limits_{x\rightarrow 2} x)^4=2^4=16$

### 問題B. $\lim\limits_{x\rightarrow 2} (x^2+2x-3)$ の極限値を求めよ．

> $=\lim\limits_{x\rightarrow 2} (x+3)(x-1)$  
> $=\lim\limits_{x\rightarrow 2} (x+3) \cdot \lim\limits_{x\rightarrow 2} (x-1)$  
> $=5\cdot 1=5$

### 問題C. $\lim\limits_{x\rightarrow 0} \frac{x^3+2x}{3x}$ の極限値を求めよ．

> $=\lim\limits_{x\rightarrow 0} (\frac{x^3}{3x}+\frac{2x}{3x})$  
> $=\lim\limits_{x\rightarrow 0} \frac{x^2}{3} +\lim\limits_{x\rightarrow 0} \frac{2}{3}$  
> $=0+\frac{2}{3}=\frac{2}{3}$

　  
　  

## 三角関数・指数関数の極限値

$\lim\limits_{\theta\rightarrow 0} \frac{\sin \theta}{\theta}=1$  
$\lim\limits_{h\rightarrow 0} \frac{e^h-1}{h}=1$  
$\lim\limits_{t\rightarrow 0} (1+t)^\frac{1}{t}$
$=\lim\limits_{x\rightarrow \pm\infty} (1+\frac{1}{x})^x=e$ 

### 問題A. $\lim\limits_{\theta\rightarrow 0} \frac{\sin \pi\theta}{\theta}$ の極限値を求めよ．

> $=\lim\limits_{\theta\rightarrow 0} \frac{\pi\sin \pi\theta}{\pi\theta}$  
> $=\pi\lim\limits_{\pi\theta\rightarrow 0} \frac{\sin \pi\theta}{\pi\theta}$  
> $=\pi\cdot 1=\pi$

<div style="page-break-before:always"></div>

### 問題B. $\lim\limits_{\theta\rightarrow 0} \frac{\theta}{\tan 3\theta}$ の極限値を求めよ．

> $=\lim\limits_{\theta\rightarrow 0} \frac{\theta}{\frac{\sin 3\theta}{\cos 3\theta}}$ $=\lim\limits_{\theta\rightarrow 0} \frac{\theta}{\sin 3\theta}\lim\limits_{\theta\rightarrow 0} \cos 3\theta$  
> $=\frac{1}{\lim\limits_{\theta\rightarrow 0} \frac{\sin 3\theta}{\theta}}\lim\limits_{3\theta\rightarrow 0} \cos 3\theta$  
> $=\frac{1}{\lim\limits_{3\theta\rightarrow 0} 3\cdot \frac{\sin 3\theta}{3\theta}}\cdot 1$ $=\frac{1}{3}\cdot 1=\frac{1}{3}$

### 問題C. $\lim\limits_{\theta\rightarrow 0} \frac{\theta\sin 3\theta}{1-\cos 3\theta}$ の極限値を求めよ．

> $=\lim\limits_{\theta\rightarrow 0} \frac{\theta\sin 3\theta(1+\cos 3\theta)}{(1-\cos 3\theta)(1+\cos 3\theta)}$ $=\lim\limits_{\theta\rightarrow 0} \frac{\theta\sin 3\theta(1+\cos 3\theta)}{1^2-\cos^2 3\theta}$  
> $=\lim\limits_{\theta\rightarrow 0} \frac{\theta\sin 3\theta(1+\cos 3\theta)}{\sin^2 3\theta}$ $=\lim\limits_{\theta\rightarrow 0} \frac{\theta(1+\cos 3\theta)}{\sin 3\theta}$  
> $=\lim\limits_{\theta\rightarrow 0} \frac{1+\cos 3\theta}{3\cdot\frac{\sin 3\theta}{3\theta}}$ $=\frac{1+\lim\limits_{3\theta\rightarrow 0} \cos 3\theta}{3\cdot\lim\limits_{3\theta\rightarrow 0} \frac{\sin 3\theta}{3\theta}}$ $=\frac{1+1}{3\cdot 1}=\frac{2}{3}$

<div style="page-break-before:always"></div>

## 微分係数（変化率）

$f'(a)=\lim\limits_{x\rightarrow a} \frac{f(x)-f(a)}{x-a}$ $=\lim\limits_{h\rightarrow 0} \frac{f(a+h)-f(a)}{h}$

### 問題A. $f(x)=x^3$ の $x=1$ における微分係数を求めよ．

> $\lim\limits_{x\rightarrow 1} \frac{x^3-1^3}{x-1}$ $=\lim\limits_{x\rightarrow 1} \frac{(x-1)(x^2+x+1)}{x-1}$  
> $=\lim\limits_{x\rightarrow 1} (x^2+x+1)$  
> $=\lim\limits_{x\rightarrow 1} x^2+\lim\limits_{x\rightarrow 1} x+1$ $=3$

### 問題B. $f(x)=\sqrt{x}$ の $x=4$ における微分係数を求めよ．

> $\lim\limits_{x\rightarrow 4} \frac{\sqrt{x}-\sqrt{4}}{x-4}$ $=\lim\limits_{x\rightarrow 4} \frac{\sqrt{x}-2}{(\sqrt{x}-2)(\sqrt{x}+2)}$  
> $=\lim\limits_{x\rightarrow 4} \frac{1}{\sqrt{x}+2}$ $=\frac{1}{\lim\limits_{x\rightarrow 4} \sqrt{x}+2}$  
> $=\frac{1}{2+2}=\frac{1}{4}$

### 問題C. $f(x)=x^2-x$ の $x=1$ における微分係数を求めよ．

> $\lim\limits_{x\rightarrow 1} \frac{x^2-x-(1^2-1)}{x-1}$  
> $=\lim\limits_{x\rightarrow 1} \frac{x^2-x}{x-1}$ $=\lim\limits_{x\rightarrow 1} \frac{x(x-1)}{x-1}$  
> $=\lim\limits_{x\rightarrow 1} x=1$  

## 導関数

$f'(x)=\lim\limits_{X\rightarrow a} \frac{f(X)-f(x)}{X-x}$ $=\lim\limits_{h\rightarrow 0} \frac{f(x+h)-f(x)}{h}$

### 問題A. $y=x^2-x$ の導関数を求めよ．

> $\lim\limits_{h\rightarrow 0} \frac{(x+h)^2-(x+h)-(x^2-x)}{h}$ $=\lim\limits_{h\rightarrow 0} \frac{1}{h}(x^2+2hx+h^2-x-h-x^2+x)$  
> $=\lim\limits_{h\rightarrow 0} \frac{1}{h}(2hx+h^2-h)$ $=\lim\limits_{h\rightarrow 0} (2x+h-1)$  
> $=2x+\lim\limits_{h\rightarrow 0} h-1=2x-1$

### 問題B. $y=x^3+2$ の導関数を求めよ．

> $\lim\limits_{h\rightarrow 0} \frac{(x+h)^3+2-(x^3+2)}{h}$ $=\lim\limits_{h\rightarrow 0} \frac{1}{h}(3hx^2+3h^2x+h^3)$  
> $=\lim\limits_{h\rightarrow 0} (3x^2+3hx+h^2)$  
> $=3x^2+\lim\limits_{h\rightarrow 0} 3hx+\lim\limits_{h\rightarrow 0} h^2$ $=3x^2$

<div style="page-break-before:always"></div>

## 導関数の性質

$(c)'=0$，$(cf)'=cf'$，$(f\pm g)'=f'\pm g'$  
$(fg)'=f'g+fg'$  
$(\frac{f}{g})'=\frac{f'g-fg'}{g^2}$  
$\{f(ax+b)\}'=af'(ax+b)$

（よく使う公式： $(x^r)'=rx^{r-1}$）

### 問題A. $y=x^4-2x^3+x$ を微分せよ．

> $y'=4x^3-2\cdot 3x^2+1$  
> 　$=4x^3-6x^2+1$

### 問題B. $y=\frac{2}{3}x^3+\frac{1}{2}x-1$ を微分せよ．

> $y'=\frac{2}{3}\cdot 3x^2+\frac{1}{2}$  
> 　$=2x^2+\frac{1}{2}$

### 問題C. $y=(x+1)(x^2-x+1)$ を微分せよ．

> $y=x^3-x^2+x+x^2-x+1$  
> 　$=x^3+1$ よって $y'=3x^2$

<div style="page-break-before:always"></div>

## 導関数の公式

$(x^r)'=rx^{r-1}$  
$(\sin x)'=\cos x$，$(\cos x)'=-\sin x$，$(\tan x)'=\frac{1}{\cos^2 x}$  
$(e^x)'=e^x$，$(a^x)'=a^x\log a$

### 問題A. $y=\sin(2-3x)$ を微分せよ．

> $y'=(\sin (-3x+2))'$  
> （導関数の性質の4番目より）  
> 　$=-3\sin'(-3x+2)$ $=-3\cos(2-3x)$

### 問題B. $y=\tan(x-2)$ を微分せよ．

> $y'=(\tan (x-2))'$  
> 　$=\tan' (x-2)$
> 　$=\frac{1}{\cos^2 (x-2)}$

### 問題C. $y=e^{2x+5}$ を微分せよ．

> （導関数の性質の4番目より）  
> $y'=2e^{2x+5}$

<div style="page-break-before:always"></div>

---

この資料と解答はwebで公開しています：  
![](../QRcode.png)  
**情報工学科のサイト（「大分高専 情報」で検索）→ スタッフ紹介（教職員紹介） → 西村俊二 → 一番下のリンク → 2S ALH**

---

解説及び問題は下記より：  
　高遠節夫他，「新微分積分I問題集」，大日本図書
