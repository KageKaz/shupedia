---
date: 2024-07-20
---
> [!definition] 
> $\vec{a}\cdot \vec{b}=\|\vec{a}\|\|\vec{b}\|\cos \theta=a_{x}b_{x}+a_{y}b_{y}$

$\| \vec{a}\| \cos \theta$ is just equal to the $\vec{b}$ component of $\vec{a}$. You take the pieces of the [[vector|vectors]] that are in the same direction and multiply them.
Dot product results in a scalar, it essentially tells you how much two [[vector|vectors]] point together

## proof of$\|\vec{a}|\|\vec{b}\|\cos \theta=a_{x}b_{x}+a_{y}b_{y}$ 
> [!todo]
> not sure this proof is good

$\vec{a}\!\cdot\!\vec{a}=\|\vec{a}\|\|\vec{a}\|\cos0$, therefore the [[dot product]] of two of the same [[vector|vectors]] is just the magnitude of that [[vector]] squared.
![[Pasted image 20240719190915.png|300]]
by the [[law of cosines]], $\|\vec{b}-\vec{a}\|^2=\| \vec{a}\|^2+\|\vec{b}\|^2-2\|\vec{a}\|\!\cdot\!\| \vec{b}\|\cos \theta$
$$
\begin{align}
2\|\vec{a}\|\!\cdot\!\| \vec{b}\|\cos \theta=&\| \vec{a}\|^2+\|\vec{b}\|^2-\|\vec{b}-\vec{a}\|^2 \\ \\
\vec{a}\!\cdot\!\ \vec{b}=&\frac{\| \vec{a}\|^2+\|\vec{b}\|^2-\|\vec{b}-\vec{a}\|^2}{2} \\
\vec{a}\!\cdot\!\ \vec{b}=&\frac{a_{x}^2+a_{y}^2+b_{x}^2+b_{y}^2-(b_{x}-a_{x})^2-(b_{y}-a_{y})^2}{2} \\&&\text{by pythagorean theorem} \\
\vec{a}\!\cdot\!\ \vec{b}=&\frac{a_{x}^2+a_{y}^2+b_{x}^2+b_{y}^2-b_{x}^2+2b_{x}a_{x}-a_{x}^2-b_{y}^2+2b_{y}a_{y}-a_{y}^2}{2}  \\
\vec{a}\!\cdot\!\ \vec{b}=&\frac{2b_{x}a_{x}+2b_{y}a_{y}}{2} \\
\vec{a}\!\cdot\!\ \vec{b}=&b_{x}a_{x}+b_{y}a_{y}


\end{align}
$$
