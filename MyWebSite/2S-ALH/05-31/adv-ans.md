
<!-- > pandoc adv-ans.md --mathjax -c ../../css/mathjax.css --include-in-header=../in-header.txt --include-before-body=../before-body.txt --include-after-body=../after-body.txt -s -o adv-ans.html -->

**2S-ALH @2017/05/31 “いろいろな関数の導関数”**

# Advanced問題

### 問題A. $y=\frac{1}{\sqrt[3]{(2-x)^2}}$ を微分せよ．

> $y=(2-x)^{-\frac{2}{3}}$ なので，  
> $y'=-\frac{2}{3}(2-x)^{-\frac{5}{3}}\cdot(-1)$  
> $=\frac{2}{3\sqrt[3]{(2-x)^5}}$  
> $=\frac{2}{3(2-x)\sqrt[3]{(2-x)^2}}$

### 問題B. $y=\log_7 (3x+1)$ を微分せよ．

> $y=\frac{\log(3x+1)}{\log 7}$  
> $y'=\frac{1}{\log 7}\cdot\frac{1}{3x+1}\cdot 3$  
> $=\frac{3}{\log 7\cdot (3x+1)}$

### 問題C. $y=x^2\sqrt{\frac{1+x^2}{1-x^2}}$ を対数微分法で微分せよ．

> $y=x^2(1+x^2)^\frac{1}{2}(1-x^2)^{-\frac{1}{2}}$  
> $\log y=\log x^2+\log(1+x^2)^\frac{1}{2}+\log (1-x^2)^{-\frac{1}{2}}$  
> $=2\log x+\frac{1}{2}\log (1+x^2)+(-\frac{1}{2}\log (1-x^2)$  
> $\frac{1}{y}y'=\frac{2}{x}+\frac{1}{2}\frac{1}{1+x^2}2x-\frac{1}{2}\frac{1}{1-x^2}(-2x)$  
> $=2x^{-1}+x(1+x^2)^{-1}+x(1-x^2)^{-1}$  
> $y'=2x^{-1}x^2(1+x^2)^\frac{1}{2}(1-x^2)^{-\frac{1}{2}}$ $+x(1+x^2)^{-1}x^2(1+x^2)^\frac{1}{2}(1-x^2)^{-\frac{1}{2}}$ $+x(1-x^2)^{-1}x^2(1+x^2)^\frac{1}{2}(1-x^2)^{-\frac{1}{2}}$  
> $=2x(1+x^2)^\frac{1}{2}(1-x^2)^{-\frac{1}{2}}$ $+x^3(1+x^2)^{-\frac{1}{2}}(1-x^2)^{-\frac{1}{2}}$ $+x^3(1+x^2)^\frac{1}{2}(1-x^2)^{-\frac{3}{2}}$  
> $=2x(1+x^2)^{-\frac{1}{2}}(1-x^2)^{-\frac{3}{2}}$ $\{(1+x^2)(1-x^2)+\frac{x}{2}(1-x^2)+\frac{x^2}{2}(1+x^2)\}$  
> $=2x(1+x^2)^{-\frac{1}{2}}(1-x^2)^{-\frac{3}{2}}$ $(x^6-x^4+1)$  
> $=\frac{2x(x^6-x^4+1)}{\sqrt{1+x^2}\sqrt{(1-x^2)^{3}}}$

### 問題D. $y=\sin^{-1} \frac{x}{\sqrt{1+x^2}}$ を微分せよ．

> $y'=\frac{1}{\sqrt{1-\frac{x^2}{1+x^2}}}\cdot\{(1+x^2)^{-\frac{1}{2}}+x(-\frac{1}{2})(1+x^2)^{-\frac{3}{2}}\cdot 2x\}$  
> $=\frac{1}{\sqrt{\frac{1+x^2-x^2}{1+x^2}}}\{\frac{1}{\sqrt{1+x^2}}-\frac{x^2}{\sqrt{(1+x^2)^3}}\}$  
> $=\sqrt{1+x^2}\cdot\{\frac{1}{\sqrt{1+x^2}}-\frac{x^2}{\sqrt{1+x^2}(1+x^2)}\}$  
> $=1-\frac{x^2}{1+x^2}$ $=\frac{1+x^2-x^2}{1+x^2}$ $=\frac{1}{1+x^2}$

---

問題は下記より：  
　高遠節夫他，「新微分積分I問題集」，大日本図書
