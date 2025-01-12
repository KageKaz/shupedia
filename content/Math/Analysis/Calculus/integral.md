---
date: 2024-12-27
aliases:
  - integrals
---
There are two ways of thinking about integrals: as a Riemann sum and as an anti-derivative.
# As a Riemann sum (definition of definite integral)
Imagine we are trying to find the [[area]] under a [[function]] over a given interval. If the function was flat, it would be simple. But if what if the function is curved? We can approximate the function with discrete tiny steps, find the [[area]] under each step, and sum them for an approximation. And as the size of the step approaches $0$ and the number of steps approaches $\infty$, we approach a perfect, approximated area. Symbolically, the [[area]] is equal to
$$
\int_{a}^{b} f(x) \,  dx= \lim_{ n \to  \, \infty  } \sum_{i=1}^nf(x_{i})\Delta x
$$
Here, $a$ and $b$ bound the interval. $\Delta x=\frac{b-a}{n}$ and $x_{i}=a+\Delta x\!\cdot\!i$
# As an anti-derivative (indefinite integral)
If taking the [[derivative]] of a position function gets us [[velocity]], then taking the anti-derivative of a velocity [[function]] gives us position. Symbolically, we represent this as an indefinite integral. 
$$
\int f(x) \, dx=F(x)+C 
$$

^dd7a97

where $F(x)$ is an anti-derivative of $f(x)$
the reason we need $+C$ is because taking the [[derivative]] of a constant gives you zero, which means there is an infinite number of possible anti-derivatives, functions where if you take the derivative of it, you get $f(x)$. Intuitively, an infinite number of position functions shifted up or down can have the same [[velocity]] at every point.
