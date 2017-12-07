
<!-- > pandoc adv-ans.md --mathjax -c ../../css/mathjax.css --include-in-header=../in-header.txt --include-before-body=../before-body.txt --include-after-body=../after-body.txt -s -o adv-ans.html -->

# 関数の極限と導関数

### 問題A. $\lim\limits_{x\rightarrow \infty} (\sqrt{x+4}-\sqrt{x})$

> $=\lim\limits_{x\rightarrow \infty} \frac{(\sqrt{x+4}-\sqrt{x})(\sqrt{x+4}+\sqrt{x})}{\sqrt{x+4}+\sqrt{x}}$  
> $=\lim\limits_{x\rightarrow \infty} \frac{x+4-x}{\sqrt{x+4}+\sqrt{x}}$   
> $=\frac{4}{\lim\limits_{x\rightarrow \infty} (\sqrt{x+4}+\sqrt{x})}$  
> $=0$

### 問題B. $\lim\limits_{h\rightarrow 0} (1+h)^{-\frac{1}{h}}$ の極限値を求めよ．

> $=\lim\limits_{h\rightarrow 0} \{(1+h)^\frac{1}{h}\}^{-1}$  
> $=\{\lim\limits_{h\rightarrow 0} (1+h)^\frac{1}{h}\}^{-1}$  
> $=e^{-1}=\frac{1}{e}$

### 問題C. $f(x)=x^2+x$ の $x=a$ における微分係数 $f'(a)$ を定義に従って求めよ．

> $\lim\limits_{h\rightarrow 0} \frac{(a+h)^2+(a+h)-(a^2+a)}{h}$  
> $=\lim\limits_{h\rightarrow 0} \frac{1}{h}(a^2+2ha+h^2+a+h-a^2-a)$  
> $=\lim\limits_{h\rightarrow 0} \frac{1}{h}(2ha+h^2+h)$  
> $=\lim\limits_{h\rightarrow 0} (2a+h+1)$  
> $=2a+\lim\limits_{h\rightarrow 0} h+1=2a+1$

### 問題D. $y=\frac{3x-1}{x^2-5}$ を微分せよ．

> $y'=\frac{(3x-1)'(x^2-5)-(3x-1)(x^2-5)'}{(x^2-5)^2}$  
> 　$=\frac{3(x^2-5)-2x(3x-1)}{(x^2-5)^2}$  
> 　$=\frac{3x^2-15-6x^2+2x}{(x^2-5)^2}$  
> 　$=\frac{-3x^2+2x-15}{(x^2-5)^2}$

### 問題E. $y=2^{-x+1}$ を微分せよ．

> 公式より $(2^x)'=2^x\log 2$ であるので，  
> $y'=-2^{-x+1}\log 2$

---

問題は下記より：  
　高遠節夫他，「新微分積分I問題集」，大日本図書
