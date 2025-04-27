---
title: AT-SW
date: 2025-02-22 02:11:39
tags:
---

我们写出 Stiefel-Whitney 满足的四条公理：

- 对每个秩 $k$ 丛 $E\to B$， 都有 $w_i(E)\in H^i(B;\mathbb Z_2),1\le i\le k$
  - 并且记 $w(E)=1+w_1(E)+w_2(E)+\cdots\in H^\bullet(B;\mathbb Z_2)$.
  - 进一步记 $w(B)=w(TB)$.
- 自然性公理：对丛映射 $f:E\to F$，有 $f^*w(F)=w(E)$.
- Whitney 加法公理：$w(E\oplus F)=w(E)\smile w(F)$.
- 正则公理：$w(\gamma\to\mathbb RP^1)=1+\alpha$.

由公理马上可得

- 对平凡丛 $\varepsilon^k\to B$ 根据自然性有 $w(\varepsilon^k)=0$.
- 若 $E$ 存在 $l$ 个线性无关截面，即 $E$ 可裂出一个秩 $l$ 平凡丛，则由加法公理有 $w_k(E)=\cdots=w_{k-l+1}(E)=0$.

我们希望计算 $w(\mathbb RP^n)$. 由于
$$T\mathbb RP^n\oplus N\mathbb RP^n\cong\hom(\gamma,\gamma^\perp)\oplus\hom(\gamma,\gamma)\cong\hom(\gamma,\varepsilon^{n+1})\cong\hom(\gamma,\varepsilon^1)^{\oplus(n+1)}\cong\gamma^{\oplus(n+1)}$$
故由于法丛平凡， $w(\mathbb RP^n)=(1+\alpha)^{n+1}$.

若有浸入 $M\subset\mathbb R^n$，则 $w(M)=w^{-1}(NM)$，进一步分析 $w^{-1}(\mathbb RP^n)$ 可得若 $\mathbb RP^{2^r}$ 浸入 $\mathbb R^{2^r+k}$，则 $k\ge 2^r-1$，Whitney 嵌入实现了这个界。

**备考.**  Smale-Hirsch, h-principle

我们定义 Stifel-Whitney 数为 $w_1^{r_1}\cdots w_n^{r_n}(E)=\langle w_1^{r_1}(E)\cdots w_n^{r_n}(E),[B]\rangle\in\mathbb Z_2$，其中 $r_1+2r_2+\cdots+nr_n=k$. 这是著名的配边不变量，因为有

**定理** (Pontryagin-Thom). $M$ 能够成为边界 $\iff$ $M$ 的 SW 数全部消失。

注意到 $w_I(\mathbb RP^{2k-1})=0$，理由是 $\mathbb RP^2$ 没有奇数次的 SW 类.

任何一个 $M\amalg M$ 也会导致 $w_I=0$.