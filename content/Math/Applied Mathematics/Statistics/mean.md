---
aliases:
  - average
  - averaging
  - means
date: 2024-12-27
---
The mean is a balancing point. The total distance from points above the mean is equal to the total distance of points below the mean. 
Mean is bad at estimating the center of skewed [[distribution]] because it is pulled by the long tail.
## population mean
$$
\mu=\frac{\sum_{i=1}^Nx_{i}}{N}
$$
## sample mean
$$
\bar{x}=\frac{\sum_{i=1}^nx_{i}}{n}
$$
# average value of a [[function]] 
the average height of a function $f(x)$ from $f(a)$ to $f(b)$ is intuitively
$$
\begin{align}
\text{average height} & =\frac{\text{area}}{\text{width}} \\
 & =\frac{\int_{a}^{b} f(x) \, dx }{b-a}
\end{align}

$$

^c865d8

mathematically
$$
\begin{align}
\text{average height} & =\frac{\text{height of samples}}{\text{number of samples}} \\
 & =\frac{\text{height of samples}}{\frac{b-a}{dx}} \\
 & =\frac{\text{height of samples }(dx)}{b-a} \\
 & =\frac{\int_{a}^{b} f(x) \, dx }{b-a}
\end{align}
$$