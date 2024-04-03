---
aliases:
  - random variables
---
> [!definition]
> A random variable represents the outcome of a random process

The [[probability distribution]] of a random variable gives its possible values and their [[probability|probabilities]].

## discrete random variables
> [!definition]
> discrete random variables take up a fixed number of possible values

> [!example]
> + the number of heads in three coin tosses
> + [[binomial variable]]
> + [[geometric variable]]
> 
#### [[mean]]
The [[mean]] ([[expected value]]) is given by the weighted [[mean|average]] of all the possible values. This is what the average value would approach for infinite trials.
$$
\mu_{X}=E(X)=\sum x_{i}p_{i}
$$
The [[mean]] of the sum or difference of [[random variable|random variables]] is the same as adding or subtracting the [[mean|means]] of the two [[random variable|random variables]] 
#### [[ standard deviation]]
The [[variance]]  is the weighted [[mean|average]] of the squared differences of each possible value from the [[mean]]. ^c893cd
$$
\sigma^2_{X}=\sum (x_{i}-\mu_{X})^2
p_{i}$$
take the square root to find [[standard deviation]] 
$$
\sigma_{X}=\sqrt{ \sum (x_{i}-\mu_{X})^2 p_{i}}
$$
The [[variance]] of the sum and difference of two [[independent]] [[random variable|random variables]] is equal to the sum of the [[variance|variances]]. ^60a6fa
> [!warning]-
> When you add [[variance|variances]], make sure they are [[independent]], otherwise they can influence each other and change the [[variance]].

> [!question]- Why not subtract the [[variance|variances]]?
> Conceptually, because [[variance]] deals with spread, subtracting [[variance|variances]] should increase it. It is always positive because it is squared. Mathematically, 
>$$
\begin{align}
\sigma_{X-Y}^2 = \sigma_{X+(-Y)}^2 &=\sigma^2_{X}+\sigma^2_{-Y} \\
\sigma_{-Y}^2&=\sum (-Y_{i}-\mu_{Y})^2p_{i} \\
\sigma_{-Y}^2&=\sum (-1)^2(Y_{i}+\mu_{Y})^2p_{i} &&\text{factor out} -1\\
\sigma_{-Y}^2&=\sum (Y_{i}+\mu_{Y})^2p_{i} &&-1^2=1\\
\sigma_{-Y}^2&=\sigma_{Y}^2 \\
\sigma_{X-Y}^2 &= \sigma^2_{X}+\sigma^2_{Y}
\end{align}
$$



## transformations
#### addition/subtraction
The [[distribution]] just gets shifted left or right by how much you add.
Thus, the [[mean]] gets larger/smaller by how much you add.
[[standard deviation]] does not change because you don't change the shape/[[variability|variation]] of the [[distribution]].
#### multiplication/division
The [[distribution]] gets stretched/compressed, changing both [[mean]] and [[standard deviation]].
Both [[mean]] and [[standard deviation]] get multiplied/divided by what you multiplied/divided the [[distribution]] by.