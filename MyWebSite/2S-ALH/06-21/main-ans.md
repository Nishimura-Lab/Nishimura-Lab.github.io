
<!-- > pandoc main-ans.md --mathjax -c ../../css/2s-alh.css --include-in-header=../in-header.txt --include-before-body=../before-body.txt --include-after-body=../after-body.txt -s -o main-ans.html -->

**2S-ALH @2017/06/21 “微積 中間試験範囲の復習”**

# 関数の極限

試験問題： $\lim\limits_{x\rightarrow \infty} \frac{2^x+3^x}{2^x-3^x}$ を計算せよ．

- このままでは分母分子ともに $\infty$ になるので計算できない
- 分母分子に何かを掛けて変形する手がある
- 何を掛けるか考えると，ここに現れている数は $2^x$ と $3^x$ ．
- 分母分子にこれらを掛けても変わらず $\infty$ なので，割ることにする
- $2^x$ で割っても $\infty$ が残りそう
- ∴ $3^x$ で割ることにする

$\lim\limits_{x\rightarrow \infty} \frac{2^x+3^x}{2^x-3^x}$
$=\lim\limits_{x\rightarrow \infty} \frac{\frac{2^x+3^x}{3^x}}{\frac{2^x-3^x}{3^x}}$
$=\lim\limits_{x\rightarrow \infty} \frac{\frac{2^x}{3^x}+1}{\frac{2^x}{3^x}-1}$  
$=\lim\limits_{x\rightarrow \infty} \frac{(\frac{2}{3})^x+1}{(\frac{2}{3})^x-1}$
$=\frac{\lim\limits_{x\rightarrow \infty} (\frac{2}{3})^x+1}{\lim\limits_{x\rightarrow \infty} (\frac{2}{3})^x-1}$
$=\frac{0+1}{0-1}$
$=-1$  

### 練習問題A. $\lim\limits_{x\rightarrow \infty} \frac{4x^2+3x+2}{3x^2+2}$ を計算せよ．

> $=\lim\limits_{x\rightarrow \infty} \frac{\frac{4x^2+3x+2}{x^2}}{\frac{3x^2+2}{x^2}}$
> $=\lim\limits_{x\rightarrow \infty} \frac{4+\frac{3}{x}+\frac{2}{x^2}}{3+\frac{2}{x^2}}$  
> $=\frac{4+3\lim\limits_{x\rightarrow \infty} \frac{1}{x}+2\lim\limits_{x\rightarrow \infty} \frac{1}{x^2}}{3+2\lim\limits_{x\rightarrow \infty} \frac{1}{x^2}}$  
> $=\frac{4+0+0}{3+0}$
> $=\frac{4}{3}$

### 練習問題B. $\lim\limits_{x\rightarrow \infty} \frac{(x+5)(2x-3)(3-x)}{x^3+2x}$ を計算せよ．

> $=\lim\limits_{x\rightarrow \infty} \frac{\frac{(x+5)(2x-3)(3-x)}{x^3}}{\frac{x^3+2x}{x^3}}$
> $=\lim\limits_{x\rightarrow \infty} \frac{\frac{x+5}{x}\frac{2x-3}{x}\frac{3-x}{x}}{1+\frac{2}{x^2}}$  
> $=\lim\limits_{x\rightarrow \infty} \frac{(1+\frac{5}{x})(2-\frac{3}{x})(\frac{3}{x}-1)}{1+\frac{2}{x^2}}$
> $=\frac{(1+5\lim\limits_{x\rightarrow \infty} \frac{1}{x})(2-3\lim\limits_{x\rightarrow \infty} \frac{1}{x})(3\lim\limits_{x\rightarrow \infty} \frac{1}{x}-1)}{1+2\lim\limits_{x\rightarrow \infty} \frac{1}{x^2}}$  
> $=\frac{(1+0)(2-0)(0-1)}{1+0}$
> $=-2$

<div style="page-break-before:always"></div>

# 導関数1

試験問題： $y=\frac{1+2^{-x}}{1+2^x}$ を微分せよ．

$(\frac{f}{g})'=\frac{f'g-fg'}{g^2}$ ，$(a^x)'=a^x\log a$ なので，  
$y'=\frac{1}{(1+2^x)^2}(-2^{-x}\log 2\cdot (1+2^x)-(1+2^{-x})\cdot2^x\log 2)$  
$=\frac{1}{(1+2^x)^2}(-2^{-x}\log 2-2^{-x}2^x\log 2-2^x\log 2-2^{-x}2^x\log 2)$  
$=\frac{1}{(1+2^x)^2}(-2^x\log 2-2^{-x}\log 2-2\log 2)$  
$=\frac{-\log 2}{(1+2^x)^2}(2^x+2^{-x}+2)$  
$=\frac{-\log 2}{(1+2^x)^2}\frac{(2^x)^2+1+2\cdot 2^x}{2^x}$  
$=\frac{-\log 2}{(1+2^x)^2}\frac{(2^x+1)^2}{2^x}$  
$=-\frac{\log 2}{2^x}$

### 問題A. $y=3^{2x+3}$ を微分せよ．

> $y'=2\cdot3^{2x+3}\log 3$  
> 　  
> 　

### 問題B. $y=\frac{3x-1}{x^2-5}$ を微分せよ．

> $y'=\frac{(3x-1)'(x^2-5)-(3x-1)(x^2-5)'}{(x^2-5)^2}$  
> $=\frac{3(x^2-5)-2x(3x-1)}{(x^2-5)^2}$  
> $=\frac{3x^2-15-6x^2+2x}{(x^2-5)^2}$  
> $=\frac{-3x^2+2x-15}{(x^2-5)^2}$

<div style="page-break-before:always"></div>

# 導関数2

試験問題： $y=\log \frac{(x+1)^2}{x(x-1)}$ を微分せよ．

$y=\log (x+1)^2x^{-1}(x-1)^{-1}$ と表し，  
$y'=\frac{1}{(x+1)^2x^{-1}(x-1)^{-1}}\{ 2(x+1)x^{-1}(x-1)^{-1} +$
$(x+1)^2x^{-2}(x-1)^{-1}+(x+1)^2x^{-1}(-(x-1)^{-2})$  
$=$…  
…とやると大変．

なので，$y=2\log (x+1)-\log x-\log(x-1)$ と表し，  
$y'=\frac{2}{x+1}-\frac{1}{x}-\frac{1}{x-1}$  
$=\frac{2x(x-1)-(x+1)(x-1)-x(x+1)}{x(x+1)(x-1)}$  
$=\frac{2x^2-2x-x^2+1-x^2-x}{x(x+1)(x-1)}$  
$=\frac{-3x+1}{x(x+1)(x-1)}$  

### 問題A. $y=\log_7 (3x+1)$ を微分せよ．

> $y=\frac{\log(3x+1)}{\log 7}$  
> $y'=\frac{1}{\log 7}\cdot\frac{1}{3x+1}\cdot 3$  
> $=\frac{3}{\log 7\cdot (3x+1)}$  
> 　

### 問題B. $y=\log(x+\sqrt{x^2+1})$ を微分せよ．

> $y'=\frac{1}{x+\sqrt{x^2+1}}(1+\frac{1}{2}\cdot\frac{2x}{\sqrt{x^2+1}})$  
> $=\frac{1}{x+\sqrt{x^2+1}}(\frac{\sqrt{x^2+1}+x}{\sqrt{x^2+1}})$  
> $=\frac{1}{\sqrt{x^2+1}}$  
> 　

<div style="page-break-before:always"></div>

この資料と解答はwebで公開しています：  
![](../QRcode.png)  
**情報工学科のサイト（「大分高専 情報」で検索）→ スタッフ紹介（教職員紹介） → 西村俊二 → 一番下のリンク → 授業 → 2S ALH**

---

解説及び問題は下記より：  
　高遠節夫他，「新微分積分I問題集」，大日本図書
