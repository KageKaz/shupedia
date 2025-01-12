---
date: 2024-12-24
---
> [!definition]
> For the quotient of two [[function|functions]] $\frac{f(x)}{g(x)}$ at a point $a$ where $f(a)\text{ and }g(a)=0$,
> $$ \lim_{ x \to a }\frac{f(x)}{g(x)}=\frac{f'(x)}{g'(x)}$$

# Intuition
Even though the ratio is not defined at $a$, it is defined at a point slightly larger than $a$, say a nudge $dx$ away. And as $dx$ gets smaller, this approximation gets better and better. The ratio $dx$ away from $a$ is
$$
\frac{\frac{df}{dx}(a)dx}{\frac{dg}{dx}(a)dx}=\frac{\frac{df}{dx}(a)}{\frac{dg}{dx}(a)}
$$
