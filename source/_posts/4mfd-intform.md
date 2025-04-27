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
定义为同调相交数，也即相交形式之名来历。早先的工作指出

**定理(Whitehead-Milnor)** 两个四流形同伦等价等价于具有相同相交形式。

</br></br>

对四维流形论而言，什么样的幺模二次型可以实现为相交形式是个很自然的问题。拓扑四流形的情形已被 Freedman 解答：

**定理** (Freedman). 对所有幺模二次型 $Q$，均存在单连通有向拓扑四流形 $X$ 使得 $Q_X\cong Q$. 
- 若 $Q$ 为偶型，每个同构类恰好对应一个胚形。
- 若 $Q$ 为奇型，每个同构类恰好被两个胚形实现，且至少一个胚形不存在光滑结构。

**推论**. 若两个单连通有向光滑四流形具有相同的相交形式，则它们必同胚。

奇型对应的两个胚形可以通过 Kirby-Siebenmann 不变量来区分，即考察 $X\times S^1$ 是否可光滑化。

**定理** (Wall). 对单连通有向闭光滑四流形 $M,N$ ，若它们的相交形式同构，那么存在 $k\ge0$ 使得 $M\#k(S^2\times S^2)$ 与 $N\#k(S^2\times S^2)$ 光滑同胚。

证明以及 $k$ 的确定要用到 Donaldson's polynomials.

</br></br>

但是二次型的光滑实现则完全不简单。对定号二次型，我们有非常简单的分类

**定理** (Donaldson). 令 $X$ 为有向闭光滑四流形。若 $Q_X$ 负定，则 $Q_X$ 可对角化成 $diag(-1,\cdots)$.

Donaldson 的这个定理利用了对规范场论的深刻研究。原始论文中需要假定单连通条件，但利用 Seiberg-Witten 理论可以移除。

注意到 $E_8$ 负定、幺模、不可对角化到 $diag(-1,\cdots)$。所以根据 Freedman 和 Donaldson，存在拓扑四流形的相交形式为 $nE_8$，但不存在光滑四流形的相交形式为 $nE_8$。这说明光滑四流形和拓扑四流形之间的差别非常大。

</br></br>

对不定号的情形，我们首先有代数上的结论

**定理.** 对不定幺模二次型 $Q$：
- 若 $Q$ 为偶型，即 $Q(\alpha,\alpha)\equiv0\pmod2$，则 $Q\cong pE_8\oplus qH, b\ge 0$. 
- 若 $Q$ 为奇型，则 $Q\cong diag(1,\cdots)\oplus diag(-1,\cdots)$.

特别地，$Q$ 为偶不定形则 $\sigma(Q)\equiv 0\pmod 8$. 这里
$$H=\begin{bmatrix}0 & 1 \\ 1 & 0\end{bmatrix}$$
是双曲二次型。

</br></br>

对不定号光滑四流形的研究，一般需要考虑额外的结构。复结构的研究即代数几何。辛结构的研究一般可以类比自复结构。此外我们还经常考虑 Spin 结构和 Spin<sup>c</sup> 结构。

Spin 结构的存在性等价于第二 Stifel-Whitney 类消失，即 
$$w_2=0\in H^2(X;\mathbb Z_2)$$
由于对闭有向光滑四流形 $X$，根据吴定理
$$Q_X(\alpha,\alpha)\equiv\langle w_2(X)\smile[\alpha]^*,[X]\rangle\pmod 2$$
所以 Spin 结构导致相交形式成为偶型（可利用“Q偶型等价于0是特征元”证明单连通情形下反之亦然）。Rohlin 利用 Arf 不变量 $\frac{1}{8}(\sigma(X)-F\cdot F)\equiv Arf(X,F)\pmod 2$ 证明了偶型会施加比纯代数性质更强的限制：

**定理** (Rholin). 对偶型的闭有向单连通光滑四流形 $X$，
$$\sigma(Q_X)\equiv0\pmod{16}.$$

这实际上意味着 Spin 流形的相交形式必不能形如 $(2p+1)E_8\oplus qH$. 利用瞬子模空间，Donaldson 进一步证明了

**定理** (Donaldson). 对闭有向 Spin 光滑四流形 $X$,
- 若 $b^+(X)=1$，则 $Q_X\cong H$.
- 若 $b^+(X)=2$，则 $Q_X\cong 2H$.

什么样的四流形特征量能被辛流形实现被称作辛地理问题。

</br></br>

另一方面，注意到 $pE_8,p\neq0$ 不能被光滑流形实现，而 $H$ 可被光滑流形 $S^2\times S^2$ 实现。那么偶不定二次型的 $H$ 要占比多少才能被光滑流形实现呢？目前只观察到 K3 曲面提供了最小实现，即 $-2E_8\oplus 3H$, 这时 $b_2=22,\sigma=16$, 从而松村提出这个最小比例是 11/8.

**猜想** (松村). $\frac{11}{8}|\sigma(X)|\le b_2(X)$

针对这个猜想，古田利用 Seiberg-Witten 理论证明了最小比例超过 $\#E_8:\# H\approx1:1$.

**定理** (古田). $\frac{10}{8}|\sigma(X)|+2\le b_2(X)$