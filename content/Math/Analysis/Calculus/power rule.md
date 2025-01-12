---
date: 2024-12-17
---
> [!definition]
> $$\frac{d}{dx}[x^n]=n\!\cdot\!x^{n-1}$$
# intuition
![[Pasted image 20241217142814.png|500]]
When thinking about what $\frac{df}{dx}$ is here, as $dx$ approaches $0$, the only significant area is $3x^2$. Everything is still multiplied by $dx$ and goes to zero.  More generally, the only significant area for $x^n$ is $nx^{n-1}$
# proof
$$
\begin{align}
d(x^n)&=(x+dx)^n-x^n \\
&=x^n+nx^{n-1}dx+\text{Multiple of }dx^2-x^n&&\text{if you take one }dx \text{ and the rest }x \text{ you get the second term}  \\
&=nx^{n-1}dx+\text{Multiple of }dx \\
\frac{d(x^n)}{dx}&=nx^n-1&&\text{the multiple of }dx \text{ goes to zero}
\end{align}
$$

