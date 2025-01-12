---
date: 2024-12-27
---
# First Part ([[integral|integrals]] and [[derivative|derivatives]] are [[inverse function|inverse functions]] )
suppose
$$
s(x)=\int_{a}^{x} v(t) \, dt
$$
then
$$
\begin{align}
ds=v(x)dt \\
\frac{ds}{dt}=v(x)
\end{align}
$$
intuitively, the rate of change of an area function is the [[value]] of the function at that point. 
# Second Part (computing definite [[integral|integrals]])
suppose $F(x)$ is a position [[function]] and $f(x)$ is it's [[derivative]].
then
$$
\begin{align}
\int_{a}^{b} f(x) \, dx&=\text{chage in position} \\
&=F(b)-F(a)
\end{align}


$$
to compute this, we just need to find the anti-derivative of $f(x)$,  $F(x)$.
## perspective from [[mean|average]] value of [[function]]
![[mean#^c865d8|average]]
$$
= \frac{F(b)-F(a)}{b-a}
$$
so the [[mean|average]] value of a [[function]] is equal to the [[mean|average]] [[slope]] of it's anti-derivative. In other words, the [[mean|average]] rate of change of a position [[function]] is equal to the [[mean|average]] value of a [[velocity]] [[function]]. So instead of computing some infinite sum, we can just find the average slope of the anti-derivative, which is the average value of the [[derivative]]. 