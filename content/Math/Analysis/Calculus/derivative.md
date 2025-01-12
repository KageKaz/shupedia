---
date: 2024-12-27
aliases:
  - differentiable
  - derivatives
---
# Intuition
Imagine a [[distance]] function, $s(t)$. To compute [[mean|average]] [[velocity]], you can divide the [[distance]] traveled over a certain period of time by that period of time. To find the "instantaneous" [[velocity]], or the derivative, you can compute the change in [[distance]] over an infinitely small period of time, $\frac{ds}{dt}$ as $dt\to0$.  As $dt\to0$, $\frac{ds}{dt}$ approaches the [[slope]] of a line [[tangent]] to the [[distance]] function.
## Paradox
Change only makes sense over a period of time. What then do we make of an "instantaneous rate of change?" The way the derivative avoids this issue is by computing the rate of change as the period of time approaches 0, without actually getting there. The derivative can be though of as the "best constant approximation for the rate of change"

> [!definition]
> The derivative of a function $f$ at $x=c$ is
> $$\lim_{ h \to 0 }\frac{f(c+h)-f(c)}{h} $$
> or
> $$\lim_{ x \to c }\frac{f(x)-f(c)}{x-c} $$

If a function is differentiable, it is also [[continuous]].
# Notation
[[Joseph-Louis Lagrange|Lagrange]]'s notation: $f'$
Used with single variable [[function|functions]].
[[Gottfried Wilhelm Leibniz|Leibniz]]'s notation: $\frac{dy}{dx}$
Useful with [[integral]]s, [[differential equation]]s, and multivariable [[calculus]].
[[Sir Isaac Newton|Newton]]'s notation: $\dot{y}$
Most commonly used in real world application



# Theorems
$$
\frac{d}{dx}k=0
$$
The [[slope]] of a constant is zero and unchanging.
$$
\frac{d}{dx}[k\!\cdot\!f(x)]=k\!\cdot\!\frac{d}{dx}f(x)
$$
Remember that the derivative is just a [[limit]], and you can factor constants out of [[limit|limits]] 
$$
\frac{d}{dx}[f(x)+g(x)]=\frac{d}{dx}f(x)+\frac{d}{dx}g(x)
$$
Same idea here, the [[limit]] of a sum is the sum of the [[limit|limits]].
$$
\frac{d}{dx}[\sin(x)]=\cos(x)
$$
> [!proof]+
> $$\begin{align}
> \lim_{ x \to 0 } \frac{\sin(x)}{x}&= 1 &&\text{by the squeeze theorem} \\
> \lim_{ x \to 0 } \frac{1-\cos(x)}{x}&= 0 &&\text{can be proved algebraically}\\
> \frac{d}{dx}[\sin(x)]&=\lim_{ \Delta x \to 0 } \frac{\sin(x+\Delta x)-\sin (x)}{\Delta x}&&\text{limit definition} \\
> &=\lim_{ \Delta x \to 0 } \frac{\cos x\sin \Delta x+\sin x\cos \Delta x-\sin x}{\Delta x}&&\text{by angle addition} \\
> &=\lim_{ \Delta x \to 0 } \frac{\cos x\sin \Delta x}{\Delta x}+\frac{\sin x\cos \Delta x-\sin x}{\Delta x} \\
> &=\cos x\lim_{ \Delta x \to 0 } \frac{\sin \Delta x}{\Delta x}+-\sin x\lim_{ \Delta x \to 0 } \frac{1-\cos \Delta x}{\Delta x}&&\text{factor} \\
> &=\cos x &&\text{substiute (1) and (2)}
> \end{align} $$

> [!geometric proof]+
> Imagine a [[unit circle]] 
> ![[Pasted image 20241217165120.png|500]]
> as $d\theta\to0$, it becomes the [[hypotenuse]] of the triangle.
> the [[triangle|triangles]] are similar
> Thus, $\cos(\theta)=\frac{d(\sin \theta)}{d\theta}$

$$
\frac{d}{dx}[\cos(x)]=-\sin(x)
$$
> [!proof]+
> $$\begin{align}
 > \frac{d}{dx}\left[ \sin\left( x+\frac{\pi}{2} \right) \right]&=\cos\left( x+\frac{\pi}{2} \right)&&\text{shifting a graph doesn't change its slope} \\
> \sin\left( x+\frac{\pi}{2} \right) & =\cos x &&\text{cofunction}\\
> \cos\left( x+\frac{\pi}{2} \right) & =-\sin(x)
> \end{align}$$

$$
\frac{d}{dx}e^x=e^x
$$
> [!proof]+
> It maybe be better to just think of this as by definition. $e^x$ is defined as the function where the derivative at every point is equal to the value of that point.
> $$\begin{align}
\frac{d}{dx}[e^x] & =\lim_{dx \to 0 } \frac{e^{x+d x}-e^x}{d x}&&\text{limit definition} \\
> & =\lim_{d x \to 0 } \frac{e^{x}e^{d x}-e^x}{d x}&&\text{exponent properties} \\
> & =e^x\lim_{ dx \to 0 } \frac{e^{d x}-1}{d x}&&\text{factor} \\
> u & =e^{d x}-1 \\
> u+1 & =e^{d x} \\
>\ln(u+1)&=d x \\
>\frac{d}{dx}[e^x]&=e^x\lim_{ n\to0}\frac{u}{\ln(u+1)} \\
 > & =e^x\lim_{ n \to 0 } \frac{1}{\ln(u+1)^{\frac{1}{u}}}&&\text{multiply top and bottom by} \frac{1}{u} \\
> & =e^x \frac{1}{\ln\left( \lim_{ n \to 0 }(u+1)^{\frac{1}{u}} \right)} &&\text{limit of composite function} \\
> & =e^x\frac{1}{\ln(e)} &&\text{by definition}\\
> & =e^x
> \end{align}$$

$$
\frac{d}{dx}n^x=\ln(n)n^x
$$
> [!proof]+
> $$\frac{d}{dx}n^x=\frac{d}{dx}(e^{\ln(n)})^x=\frac{d}{dx}(e^{\ln (n)x})=\ln(n)e^{\ln(n)x}=\ln(n)n^x$$


$$
\frac{d}{dx}[\ln(x)]=\frac{1}{x}
$$
> [!proof]+
> $$\begin{align}
> y & =\ln x \\
> e^y&=x \\
> \frac{d}{dx}[e^y] & =\frac{d}{dx}[x] &&\text{implicit differentiation}\\
> e^y\!\cdot\!\frac{dy}{dx} & =1 \\
> \frac{dy}{dx}&=\frac{1}{e^y} \\
>  & =\frac{1}{e^{\ln x}} &&\text{substitute}\\
> & =\frac{1}{x}
> \end{align}$$

![[power rule]]
## combinations of [[function|functions]] 
### Adding/Subtracting
$$
\frac{d}{dx}(g(x)+h(x))=\frac{dg}{dx}+\frac{dh}{dx}
$$
### Multiplying/Dividing
$$
\frac{d}{dx}(nf(x))=n\frac{d}{dx}f(x)
$$
$$
\frac{d}{dx}[g(x)f(x)]=g(x)\frac{dh}{dx}+h(x)\frac{dg}{dx}
$$

> [!proof]+
> ![[Pasted image 20241217214743.png]]
> ![[Pasted image 20241217214045.png]]
### Composing
![[chain rule]]