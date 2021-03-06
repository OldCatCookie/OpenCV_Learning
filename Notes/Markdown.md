---
title: "Markdown"
author: tsy
date: Nov 20, 2021
output: pdf_document
---

# 一级标题

## 二级标题

### 三级标题

每写完一个段落要隔一行空行.

就像这样, 隔了一行空行.


---

分割线

**重点加粗**

*斜体*

~~删除线~~

**==高亮==**



---

列表:

* 无序列表 
  * 嵌套无序列表
  * 嵌套无序列表
* 无序列表
* 无序列表

1. 有序列表 1
   1. 嵌套有序列表 1
   2. 嵌套有序列表 2
2. 有序列表 2
3. 有序列表 3


---

引用文本:

> 引用别人说的话
> 就这样写
> By. OrangeX4

---

这是 `行内代码` 语法.

代码块语法:

``` python
print("Hello, World!")
```

请将 ' 替换成 `.

---

[超链接名称]()

![图片提示语](./image/2021-10-21-21-21-35.png)

我经常去的几个网站[Google][1]、[Leanote][2]。

[1]:http://www.google.com 
[2]:http://www.leanote.com

图片粘贴快捷键：ctrl+alt+V

---

表格:

| 表头 | 表头 |
| ---- | ---- |
| 内容 | 内容 |
| 内容 | 内容 |

---

注释:

<!-- 你看不见我 -->

---

- [x] 已经完成的事
- [ ] 未完成的事

---

注释:

<!-- 你看不见我 -->

<!-- 多行注释
就像这样 -->

---

行内公式: 

单位圆 $x^2+y^2=1$

公式块:

$$
\begin{cases}
x=\rho\cos\theta \\
y=\rho\sin\theta \\
\end{cases}
$$

---

上标 $x^2 + y^{12} = 1$

上标 $x_1 + y_{12} = 1$

---

分式

较小的行内行分数 $\frac{1}{2}$

展示型的分式 $\displaystyle\frac{x+1}{x-1}$

---

开平方 $\sqrt{2}$

开 $n$ 次方 $\sqrt[n]{2}$

---

紧贴 $a\!b$

没有空格 $ab$

小空格 $a\,b$

中等空格 $a\;b$

大空格 $a\ b$

quad 空格 $a\quad b$

两个 quad 空格 $a\qquad b$

---

累加 $\sum_{k=1}^n\frac{1}{k}  \quad  \displaystyle\sum_{k=1}^n\frac{1}{k}$

累乘 $\prod_{k=1}^n\frac{1}{k}  \quad  \displaystyle\prod_{k=1}^n\frac{1}{k}$

积分 $\displaystyle \int_0^1x{\rm d}x  \quad  \iint_{D_{xy}}  \quad  \iiint_{\Omega_{xyz}}$

---

括号修饰：用\left \rightk 可以让括号适配内部大小。

圆括号 $\displaystyle \left(\sum_{k=1}^{n}\frac{1}{k} \right)^2$

方括号 $\displaystyle \left[\sum_{k=1}^{n}\frac{1}{k} \right]^2$

花括号 $\displaystyle \left\{\sum_{k=1}^{n}\frac{1}{k} \right\}^2$

尖括号 $\displaystyle \left\langle\sum_{k=1}^{n}\frac{1}{k} \right\rangle^2$

---

多行算式对齐

居中:

$$
\begin{aligned}
y &=(x+5)^2-(x+1)^2 \\
&=(x^2+10x+25)-(x^2+2x+1) \\
&=8x+24 \\
\end{aligned}
$$

左对齐:

$
\begin{aligned}
y &=(x+5)^2-(x+1)^2 \\
&=(x^2+10x+25)-(x^2+2x+1) \\
&=8x+24 \\
\end{aligned}
$

---

方程组：

$$
\begin{cases}
k_{11}x_1+k_{12}x_2+\cdots+k_{1n}x_n=b_1 \\
k_{21}x_1+k_{22}x_2+\cdots+k_{2n}x_n=b_2 \\
\cdots \\
k_{n1}x_1+k_{n2}x_2+\cdots+k_{nn}x_n=b_n \\
\end{cases}
$$

---

矩阵:

$$
\begin{pmatrix}
1 & 1 & \cdots & 1 \\
1 & 1 & \cdots & 1 \\
\vdots & \vdots & \ddots & \vdots \\
1 & 1 & \cdots & 1 \\
\end{pmatrix}

\quad

D_{N}=\begin{bmatrix}
    1&1&1&1 \\
    1&W_{4}^1&W_{4}^2&W_{4}^3 \\
    1&W_{4}^2&W_{4}^4&W_{4}^6 \\
    1&W_{4}^3&W_{4}^6&W_{4}^9
\end{bmatrix}=\begin{bmatrix}
    1&1&1&1 \\
    1&i&-1&-i \\
    1&-1&1&-1 \\
    1&-i&-1&i
\end{bmatrix}
$$ 

行列式: 

$$
\begin{vmatrix}
1 & 1 & \cdots & 1 \\
1 & 1 & \cdots & 1 \\
\vdots & \vdots & \ddots & \vdots \\
1 & 1 & \cdots & 1 \\
\end{vmatrix}
$$

---

特殊字符

![](image/2021-10-20-15-18-38.png)

---

公式编号与引用

$$
x+2 \tag{1.2}
$$

$$
\begin{equation}
x^n+y^n=z^n
\end{equation}
$$

由公式 $(1.2)$ 可得到结论

---

### 符号的转义

在使用 markdown 编辑器编写文档的时候，有时候需要输入一些特别符号，然而却是 markdown 的语法,此时需要进行转义,即在符号前加\：

>\\\ 反斜杠
\\` 反引号
\\* 星号
\\_ 下划线
\\{\} 大括号
\\[\] 中括号
\\(\) 小括号
\\# 井号
\\+ 加号
\\- 减号
\\. 英文句号
\\! 感叹号

---

### 关系运算符

$$
1.\pm\\
2.\times\\
3.\div\\
4.\mid\\
5.\nmid\\
6.\cdot\\
7.\circ\\
8.\ast\\
9.\bigodot\\
10\bigotimes\\
11.\bigoplus\\
12.\leq\\
13.\geq\\
14.\neq\\
15.\approx\\
16.\equiv\\
17.\sum\\
18.\prod\\
19.\coprod\\
$$

--- 

<center>行中心对齐</center>
<p align="left">行左对齐</p>
<p align="right">行右对齐</p>

不同字体：

$
\rm{A}\\
\cal{A}\\
\it{A}\\
\Bbb{A}\\
\bf{A}\\
\sf{A}\\
\tt{A}\\
\frak{A}\\
\boldsymbol{A}
$

---

特殊符号：

$\vec{a}$  向量
$\overline{a}$ 平均值
$\widehat{a}$ (线性回归，直线方程) y尖
$\widetilde{a}$ 颚化符号  等价无穷小
$\dot{a}$   一阶导数
$\ddot{a}$  二阶导数

---

## 字体字号与颜色

<font face="黑体">我是黑体字</font>
<font face="微软雅黑">我是微软雅黑</font>
<font face="STCAIYUN">我是华文彩云</font>
<font color=#0099ff size=7 face="黑体">color=#0099ff size=72 face="黑体"</font>
<font color=#00ffff size=72>color=#00ffff</font>
<font color=gray size=72>color=gray</font>

![](image/2022-03-21-20-13-43.png)
![](image/2022-03-21-20-14-03.png)
![](image/2022-03-21-20-14-17.png)












