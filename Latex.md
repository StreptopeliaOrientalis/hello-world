# Latex

来源：https://www.cnblogs.com/houkai/p/3399646.html 版本3.141592

## 基础

控制序列：以"\"开头，**必须参数**{}  **可选参数**[]

数学模式有两种：文字中；单独一行

## 数学公式基本语法

[1] 上标与下标

$$x_{22}^{(n)}$$ `$$x_{22}^{(n)}$$`

$${}^*\!x*$$ `$${}^*\!x*$$`

[2] 分式

$$\frac{x+y}{2}$$ `$$\frac{x+y}{2}$$`

[3] 根式

$\sqrt{2} <\sqrt[3]{3}$   `$\sqrt{2} <\sqrt[3]{3}$`

`$\sqrt{1+\sqrt[^p\!]{1+a^2}}$`
$$
\sqrt{1+\sqrt[^p\!]{1+a^2}}
$$
`$\sqrt{1+\sqrt[^p\!]{1+a^2}}$`
$$
\sqrt{1+\sqrt[^p\!]{1+a^2}}
$$
[4] 求和`\sum`与积分`\int`

$$\sum_{k =1}^{n}\frac{1}{k}$$ `$$\sum_{k =1}^{n}\frac{1}{k}$$`

$$\int_a^b f(x)dx$$ `$$\int_a^b f(x)dx$$`

[5] 空格(beautify)

$a\!b$ `$a\!b$` 社恐的噩梦

$ab$ `$ab$`

$a\,b$ `$a\,b$`

$a\;b$ `$a\;b$`

$a\quad b$ `$a\quad b$`

$a\qquad b$ `$a\qquad b$`

[6] 定界符

[7] 矩阵

$$\begin{matrix}1 & 2\\3&4\end{matrix}$$ `$$\begin{matrix}1 & 2\\3&4\end{matrix}$$`

$\begin{pmatrix}1 & 2\\3&4\end{pmatrix} $  `$$\begin{pmatrix}1 & 2\\3&4\end{pmatrix}$$`

$\begin{Bmatrix}1 & 2\\3&4\end{Bmatrix} $  `$$\begin{Bmatrix}1 & 2\\3&4\end{Bmatrix}$$`

$\begin{vmatrix}1 & 2\\3&4\end{vmatrix} $  `$$\begin{vmatrix}1 & 2\\3&4\end{vmatrix}$$`

$\begin{Vmatrix}1 & 2\\3&4\end{Vmatrix} $  `$$\begin{Vmatrix}1 & 2\\3&4\end{Vmatrix}$$`

[8] 排版数组

矩阵的规模超过十列
$$
\mathbf{X} = 
\left( \begin{array}{ccc}
x_{11} & x_{12} & \ldots \\
x_{21} & x_{22} & \ldots \\
\vdots & \vdots & \vdots
\end{array} \right
)
$$

```latex
\mathbf{X} = 
\left( \begin{array}{ccc}
x_{11} & x_{12} & \ldots \\
x_{21} & x_{22} & \ldots \\
\vdots & \vdots & \vdots
\end{array} \right
)
```



11~35需要载入amssymb宏包并装入AMS数学字体

## 1 数学模式重音符号

$\hat{a}$  `\hat{a}`

$\check{a}$ `\check{a}`

$\tilde{a}$ `\tilde{a}`

$\grave{a}$ `\grave{a}`

$\dot{a}$ `\dot{a}`

$\ddot{a}$ `\ddot{a}`

$\bar{a}$  `\bar{a}`

$\vec{a}$ `\vec{a}`

$\widehat{a}$ `\widehat{a}`

$\acute{a}$ `\acute{a}`

$\breve{a}$ `\breve{a}`

$\widetilde{A}$`\widetilde{A}`



## 2 希腊字母

| $\alpha$      | \alpha      | $\theta$    | \theta    | $o$         | o         | $\upsilon$ | \upsilon |
| ------------- | ----------- | ----------- | --------- | ----------- | --------- | ---------- | -------- |
| $\beta$       | \beta       | $\vartheta$ | \vartheta | $\pi$       | \pi       | $\phi$     | \phi     |
| $\gamma$      | \gamma      | $\iota$     | \iota     | $\varpi$    | \varpi    | $\varphi$  | \varphi  |
| $\delta$      | \delta      | $\kappa$    | \kappa    | $\rho$      | \rho      | $\chi$     | \chi     |
| $\epsilon$    | \epsilon    | $\lambda$   | \lambda   | $\varrho$   | \varrho   | $\psi$     | \psi     |
| $\varepsilon$ | \varepsilon | $\mu$       | \mu       | $\sigma$    | \sigma    | $\omega$   | \omega   |
| $\zeta$       | \zeta       | $\nu$       | \nu       | $\varsigma$ | \varsigma |            |          |
| $\eta$        | \eta        | $\xi$       | \xi       | $\tau$      | \tau      |            |          |
| $\Gamma$      | \Gamma      | $\Lambda$   | \Lambda   | $\Sigma$    | \Sigma    | $\Psi$     | \Psi     |
| $\Delta$      | \Delta      | $Xi$        | \Xi       | $\Upsilon$  | \Upsilon  | $\Omega$   | \omega   |
| $\Theta$      | \Theta      | $\Pi$       | \Pi       | $\Phi$      | \Phi      |            |          |



## 3 二元关系

在其前面加上`\not`之后，能得到其否定形式

| $<$         | <         | $>$         | >         | $=$       | =       |
| ----------- | --------- | ----------- | --------- | --------- | ------- |
| $\le$       | \le       | $\ge$       | \ge       | $\equiv$  | \equiv  |
| $\ll$       | \ll       | $\gg$       | \gg       | $\doteq$  | \doteq  |
| $\prec$     | \prec     | $\succ$     | \succ     | $\sim$    | \sim    |
| $\preceq$   | \preceq   | $\succeq$   | \succeq   | $\simeq$  | \simeq  |
| $\subset$   | \subset   | $\supset$   | \supset   | $\approx$ | \approx |
| $\subseteq$ | \subseteq | $\supseteq$ | \supseteq | $\cong$   | \cong   |
|             |           |             |           |           |         |
|             |           |             |           |           |         |
|             |           |             |           |           |         |
|             |           |             |           |           |         |
|             |           |             |           |           |         |
|             |           |             |           |           |         |
|             |           |             |           |           |         |



## 4 二元运算符

## 5 大运算符

## 6 箭头

$\Rightarrow$ `$\Rightarrow$`

$\Longrightarrow$ `$\Longrightarrow$`

$\rightharpoonup$ `$\rightharpoonup$`

$\Leftrightarrow$   `$$\Leftrightarrow$$`

## 7 定界符

## 8 大定界符

## 9 其他符号

## 10 非数学符号

## 11 AMS定界符



$\Game$

