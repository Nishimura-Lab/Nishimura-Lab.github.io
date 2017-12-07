
<!-- > pandoc main-ans.md --mathjax -c ../../css/mathjax.css --include-in-header=../in-header.txt --include-before-body=../before-body.txt --include-after-body=../after-body.txt -s -o main-ans.html -->

**2S-ALH @2017/06/07 “平面のベクトル”**

# ベクトルの演算

$\vec{a}+\vec{b}=\vec{b}+\vec{a}$，　$(\vec{a}+\vec{b})+\vec{c}=\vec{a}+(\vec{b}+\vec{c})$

$m(n\vec{a})=(mn)\vec{a}$，　$(m+n)\vec{a}=m\vec{a}+n\vec{a}$，　$m(\vec{a}+\vec{b})=m\vec{a}+m\vec{b}$

### 問題A. 下のベクトル $\vec{PQ}$ を $\vec{a},\vec{b},\vec{c},\vec{d}$ で表せ．

![](fig1.png)

> $\vec{PQ}=\vec{d}-\vec{b}-\vec{c}+\vec{a}$

<div style="page-break-before:always"></div>

### 問題B. $3(-\vec{a}+4\vec{b})+2(2\vec{a}-5\vec{b})$ を簡単にせよ．

> $-3\vec{a}+12\vec{b}+4\vec{a}-10\vec{b}$  
> $=\vec{a}+2\vec{b}$

### 問題C. $2\vec{a}+(\vec{b}-\vec{x})=-3\vec{x}-\vec{a}+3\vec{b}$ のとき，$\vec{x}$ を $\vec{a}, \vec{b}$ で表せ．

> $2\vec{x}=-3\vec{a}+2\vec{b}$  
> $\vec{x}=-\frac{3}{2}\vec{a}+\vec{b}$

### 問題D. $|\vec{a}|=5$ のとき，$\vec{a}$ と向きが反対で大きさが $1$ のベクトルを求めよ．

> $-\frac{1}{5}\vec{a}$

<div style="page-break-before:always"></div>

# ベクトルの成分

$A(a_1,a_2),B(b_1,b_2)$ ⇒ $\vec{AB}=(b_1-a_1,b_2-a_2)$

$\vec{a}=(a_1,a_2)$ ⇒ $|\vec{a}|=\sqrt{a_1^2+a_2^2}$

### 問題A. $\vec{a}=(-2,3)$，$\vec{b}=(1,-1)$ のとき，$2\vec{a}-\vec{b}$ の大きさを求めよ．

> $2\vec{a}-\vec{b}=(-4,6)-(1,-1)$  
> 　$=(-5,7)$ ．よって，  
> $|2\vec{a}-\vec{b}|=\sqrt{(-5)^2+7^2}$ $=\sqrt{74}$

### 問題B. $\vec{a}=(-2,3)$，$\vec{b}=(1,-1)$ のとき，$\frac{1}{2}\vec{a}+\vec{b}$ の大きさを求めよ．

> $\frac{1}{2}\vec{a}+\vec{b}=(-1,\frac{3}{2})+(1,-1)$  
> 　$=(0,\frac{1}{2})$ ．よって，  
> $|\frac{1}{2}\vec{a}+\vec{b}|=\sqrt{0+(-\frac{1}{2})^2}$ $=\frac{1}{2}$

### 問題C. $A(1,-1)$，$B(3,1)$ のとき，$\vec{AB}$ の大きさを求めよ．

> $\vec{AB}=(3,1)-(1,-1)=(2,2)$  
> ∴ $|\vec{AB}|=\sqrt{2^2+2^2}$ $=2\sqrt{2}$

### 問題D. 3点 $A(-1,0), B(2,-1), C(x,y)$ と正の実数 $k$ について，$\vec{AC}=k\vec{AB}$，$|\vec{AC}|=20$ が成り立つとき，$k$ の値を求めよ．

> $\vec{AC}=k\vec{AB}$ $=k\{(2,-1)-(-1,0)\}$ $(x-1,y-1)=k(3,-1)$  
> ∴ $|\vec{AC}|=\sqrt{(3k)^2+(-k)^2}$ $=k\sqrt{10}$  
> ∴ $k=2\sqrt{10}$

<div style="page-break-before:always"></div>

# ベクトルの内積

$\vec{a}\cdot\vec{b}$ $=|\vec{a}||\vec{b}|\cos\theta$ $=a_1b_1+a_2b_2$

### 問題A. $|\vec{a}|=4, |\vec{b}|=2, \theta=\frac{\pi}{6}$ のとき，$\vec{a}$ と $\vec{b}$ の内積を求めよ．

> $4\cdot 2\cdot\cos\frac{\pi}{6}$ $=4\cdot 2\cdot\frac{\sqrt{3}}{2}$ $=4\sqrt{3}$

### 問題B. $|\vec{a}|=2, |\vec{b}|=\sqrt{3}, \theta=\frac{3}{4}\pi$ のとき，$\vec{a}$ と $\vec{b}$ の内積を求めよ．

> $2\cdot\sqrt{3}\cdot\cos\frac{3}{4}\pi$ $=2\cdot\sqrt{3}\cdot(-\frac{1}{\sqrt{2}})$ $=-\sqrt{6}$

### 問題C. $\vec{a}=(1,-3)$ と $\vec{b}=(-2,-1)$ の内積を求めよ．

> $\vec{a}\cdot\vec{b}$ $=1\cdot(-2)+(-3)\cdot(-1)$ $=1$

### 問題D. $|\vec{a}|=\sqrt{3}, |\vec{b}|=\sqrt{5}, \vec{a}\cdot\vec{b}=1$ のとき，$(2\vec{a}-\vec{b})\cdot(\vec{a}+\vec{b})$ を求めよ．

> $(2\vec{a}-\vec{b})\cdot(\vec{a}+\vec{b})$ $=2\vec{a}\cdot\vec{a}+2\vec{a}\cdot\vec{b}-\vec{a}\cdot\vec{b}-\vec{b}\cdot\vec{b}$  
> $=2\cdot 3+2-1-5=2$

<div style="page-break-before:always"></div>

# ベクトルの平行と垂直

$\vec{a}\parallel\vec{b} \Leftrightarrow \vec{b}=m\vec{a}$ を満たす $m$ が存在

$\vec{a}\perp\vec{b} \Leftrightarrow \vec{a}\cdot\vec{b}=0$

$(\vec{a}\ne0, \vec{b}\ne0)$

### 問題A. $\vec{a}=(2,k)$ と $\vec{b}=(-3,k+5)$ が平行となるように $k$ の値を定めよ．

> $(2,k)=m(-3,k+5)$  
> \begin{eqnarray} \left\{ \begin{array}{l}
>   2=-3m \\
>   k=mk+5m
> \end{array} \right. \end{eqnarray}
> ∴ $m=-\frac{2}{3}$  
> $k=-\frac{2}{3}k-\frac{10}{3}$  
> $\frac{5}{3}k=-\frac{10}{3}$  
> $k=-2$

### 問題B. $\vec{a}=(1,3)$ と $\vec{b}=(k,k+4)$ が平行となるように $k$ の値を定めよ．

> $(1,3)=m(k,k+4)$  
> \begin{eqnarray} \left\{ \begin{array}{l}
>   1=mk \\
>   3=mk+4m
> \end{array} \right. \end{eqnarray}
> $2=4m$ ∴ $m=\frac{1}{2}$  
> $1=\frac{1}{2}k$  
> ∴ $k=2$

<div style="page-break-before:always"></div>

### 問題C. $\vec{a}=(2,-1)$ と $\vec{b}=(k-1,k)$ が垂直となるように定数 $k$ の値を定めよ．

> $(2,-1)\cdot(k-1,k)=0$  
> $2k-2-k=0$  
> ∴ $k=2$

<div style="page-break-before:always"></div>

この資料と解答はwebで公開しています：  
![](../QRcode.png)  
**情報工学科のサイト（「大分高専 情報」で検索）→ スタッフ紹介（教職員紹介） → 西村俊二 → 一番下のリンク → 2S ALH**

---

解説及び問題は下記より：  
　高遠節夫他，「新線型代数問題集」，大日本図書
