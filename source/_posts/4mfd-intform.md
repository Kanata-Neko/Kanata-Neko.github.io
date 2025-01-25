---
title: 四维流形笔记#1：相交形式
date: 2025-01-21 16:01:46
tags:
---

长期随时重写， V1.0。

对一个四维拓扑流形 $X$，其同调信息 $H_\bullet(X;\mathbb Z)$ 包含些什么呢？利用万有系数定理和 Poincare 对偶，我们可以毫无障碍地列出：
$$\begin{matrix}
H^0=\mathbb Z & H^1=\mathbb Z^{b_1} & H^2=\mathbb Z^{b_2}\oplus T & H^3=\mathbb Z^{b_1}\oplus T & H^4=\mathbb Z \\
H_0=\mathbb Z & H_1=\mathbb Z^{b_1}\oplus T & H_2=Z^{b_2}\oplus T & H_3=\mathbb Z^{b_1} & H_4=\mathbb Z
\end{matrix}
$$ 
其中 $T$ 是挠，$b_1,b_2$ 是 Betti 数。注意到杯积只在
$$ \smile:H^2\times H^2\to H^4 $$
带有非平凡信息，据此我们配合上基本类得到一个整数。
$$ H^2\times H^2\to\mathbb Z:(\alpha,\beta)\mapsto\langle\alpha\smile\beta,[X]\rangle. $$
注意到双线性性，所有挠必落在零空间，从而我们一般可以杀掉挠。我们定义 $X$ 的相交形式为幺模二次型
$$ Q_X:H^2/\text{Tors}\times H^2/\text{Tors}\to\mathbb Z. $$
或者，等价地，将
$$ Q_X:H_2/\text{Tors}\times H_2/\text{Tors}\to\mathbb Z, $$
定义为同调相交数，也即相交形式之名来历。

</br></br>

对四维流形论而言，什么样的幺模二次型可以实现为相交形式是个很自然的问题。拓扑四流形的情形已被 Freedman 解答：

**定理** (Freedman). 对所有幺模二次型 $Q$，均存在单连通有向拓扑四流形 $X$ 使得 $Q_X\cong Q$. 每个同构类恰好被两个胚形实现，且至少一个胚形不存在光滑结构。

**推论**. 若两个单连通有向光滑四流形具有相同的相交形式，则它们必同胚。