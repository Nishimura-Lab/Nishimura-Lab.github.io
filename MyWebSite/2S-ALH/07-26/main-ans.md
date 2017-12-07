
<!-- > pandoc main-ans.md --mathjax -c ../../css/2s-alh.css --include-in-header=../in-header.txt --include-before-body=../before-body.txt --include-after-body=../after-body.txt -s -o main-ans.html -->

**2S-ALH @2017/07/24 “微分積分I 期末試験対策”**

# 関数の極大・極小，最大・最小

- $f'>0$ ⇒ 単調増加
- $f'<0$ ⇒ 単調減少
- $a$ で極値 ⇒ $f'(a)=0$

### 問題A. $y=x^3-6x^2+9x-3$ の極値を求めよ．

> $y'=3x^2-12x+9$
> $=3(x-1)(x-3)$  
> 　  
> <style type="text/css">
> .table1 { border-collapse: collapse; }
> .table1 td { text-align: center; }
> </style>
> <table class="table1" border=1>
>  <tr><th>$x$</th><th>…</th><th>1</th><th>…</th><th>3</th><th>…</th></tr>
>  <tr><td>$y'$</td><td>+</td><td>0</td><td>-</td><td>0</td><td>+</td></tr>
>  <tr><td>$y$</td><td>↗</td><td>1</td><td>↘</td><td>-3</td><td>↗</td></tr>
> </table>
> よって，極大値 $1$，極小値 $-3$ ．

### 問題B. $y=x^4-4x$ の極値を求めよ．

> $y'=4x^3-4$
> $=4(x^3-1)$  
> 　  
> <style type="text/css">
> .table1 { border-collapse: collapse; }
> .table1 td { text-align: center; }
> </style>
> <table class="table1" border=1>
>  <tr><th>$x$</th><th>…</th><th>1</th><th>…</th></tr>
>  <tr><td>$y'$</td><td>-</td><td>0</td><td>+</td></tr>
>  <tr><td>$y$</td><td>↘</td><td>-3</td><td>↗</td></tr>
> </table>
> よって，極大値なし，極小値 $-3$ ．

<div style="page-break-before:always"></div>

### 問題C. $y=\sin x+\cos x$ の $0\le x \le \pi$ における最大値，最小値を求めよ．

> $y'=\cos x-\sin x$  
> 　  
> <style type="text/css">
> .table1 { border-collapse: collapse; }
> .table1 td { text-align: center; }
> </style>
> <table class="table1" border=1>
>  <tr><th>$x$</th><th>0</th><th>…</th><th>$\frac{\pi}{4}$</th><th>…</th><th>$\pi$</th></tr>
>  <tr><td>$y'$</td><td></td><td>+</td><td>0</td><td>-</td><td></td></tr>
>  <tr><td>$y$</td><td>1</td><td>↗</td><td>$\sqrt{2}$</td><td>↘</td><td>-1</td></tr>
> </table>
> よって，最大値 $\sqrt{2}$ ，最小値 $-1$ ．

### 問題D. 関数 $y=-x^3+3x^2-a$ の極大値と極小値がともに負となるように，定数 $a$ の値の範囲を定めよ．

> $y'=-3x^2+6x$
> $=-3x(x-2)$  
> 　  
> <style type="text/css">
> .table1 { border-collapse: collapse; }
> .table1 td { text-align: center; }
> </style>
> <table class="table1" border=1>
>  <tr><th>$x$</th><th>…</th><th>0</th><th>…</th><th>2</th><th>…</th></tr>
>  <tr><td>$y'$</td><td>-</td><td>0</td><td>+</td><td>0</td><td>-</td></tr>
>  <tr><td>$y$</td><td>↘</td><td>-a</td><td>↗</td><td>4-a</td><td>↘</td></tr>
> </table>
> 条件は $-a<0$ ，$4-a<0$ となるので，
> $a>4$ ．

### 問題E. 関数 $y=x^3+ax^2+bx+c$ （ $a,b,c$ は定数）が $x=1$ で極大になり，$x=3$ で極小になるとき，極大値と極小値の差を求めよ．

> $y'=3x^2+2ax+b$  
> $x=1,3$ で $y'=0$ となるので，  
> \begin{eqnarray} \left\{ \begin{array}{l}
>   3+2a+b=0 \\
>   27+6a+b=0
> \end{array} \right. \end{eqnarray}
> よって，$a=-6, b=9$ ．  
> 関数は $y=x^3-6x^2+9x+c$ となり，
> $x=1$ での値と $x=3$ での値の差は，  
> $(1-6+9+c)-(27-54+27+c)$
> $=4$ ．

<div style="page-break-before:always"></div>

# 不定形の極限

**ロピタルの定理**

$\lim\limits_{x\rightarrow a} \frac{f(x)}{g(x)}=\frac{0}{0}$ か $\frac{\infty}{\infty}$ ならば，  
$\lim\limits_{x\rightarrow a} \frac{f(x)}{g(x)}=\lim\limits_{x\rightarrow a} \frac{f'(x)}{g'(x)}$  

### 問題A. $\lim\limits_{x\rightarrow 1} \frac{x^3-2x^2-3x+4}{-x^3+x^2+2x-2}$ の極限値を求めよ．

> 分子，分母ともに $0$ に収束するので，  
> $\lim\limits_{x\rightarrow 1} \frac{3x^2-4x-3}{-3x^2+2x+2}$
> $=-4$

### 問題B. $\lim\limits_{x\rightarrow 0} \frac{\log(1+x^2)}{x}$ の極限値を求めよ．

> 分子，分母ともに $0$ に収束するので，  
> $\lim\limits_{x\rightarrow 0} \frac{\frac{1}{1+x^2}\cdot 2x}{1}$
> $=\lim\limits_{x\rightarrow 0} \frac{2x}{x^2+1}$
> $=0$

### 問題C. $\lim\limits_{x\rightarrow 0} \frac{2\cos x-2+x^2}{x^4}$ の極限値を求めよ．

> 分子，分母ともに $0$ に収束するので，  
> $\lim\limits_{x\rightarrow 0} \frac{-2\sin x+2x}{4x^3}$ ．  
> まだ分子，分母ともに $0$ に収束するので，  
> $\lim\limits_{x\rightarrow 0} \frac{-2\cos x+2}{12x^2}$ ．  
> まだ分子，分母ともに $0$ に収束するので，  
> $\lim\limits_{x\rightarrow 0} \frac{2\sin x}{24x}$ ．  
> まだ分子，分母ともに $0$ に収束するので，  
> $\lim\limits_{x\rightarrow 0} \frac{2\cos x}{24}$
> $=\frac{1}{12}$

### 問題D. $\lim\limits_{x\rightarrow \infty} \sqrt[x]{x}$ の極限値を求めよ．

> $y=\lim\limits_{x\rightarrow \infty} \sqrt[x]{x}$ とすると，  
> $\log y=\log \lim\limits_{x\rightarrow \infty} {x}^\frac{1}{x}$
> $=\lim\limits_{x\rightarrow \infty} \log {x}^\frac{1}{x}$  
> $=\lim\limits_{x\rightarrow \infty} \frac{1}{x} \cdot \log {x}$
> $=\lim\limits_{x\rightarrow \infty} \frac{\log {x}}{x}$ ．  
> 分子，分母ともに $\infty$ に収束するので，  
> $\log y=\lim\limits_{x\rightarrow \infty} \frac{\frac{1}{x}}{1}$
> $=\lim\limits_{x\rightarrow \infty} \frac{1}{x}$
> $=0$  
> よって，$y=1$ ．

　  
　  
　  

---

この資料と解答はwebで公開しています：  
![](../QRcode.png)  
**西村のオフィシャルサイト（「大分高専 西村」で検索）→ 一番下のリンク → 授業 → 2S ALH**

---

解説及び問題は下記より：  
　高遠節夫他，「新微分積分I問題集」，大日本図書
