---
aliases:
  - binomial variables
date: 2024-04-02
---
* made up of a finite and fixed number of [[independent]] trials
	* we can use the [[10% rule|ten percent rule]] to establish [[independent|independence]]
* each trial can be classified as either success or failure
* probability of success on each trial is constant
> [!example]
> + How many successes in finite number of trials?
 >+ number of heads after 10 flips of a coin

the [[probability distribution]] of a binomial variable is a binomial [[distribution]]  

## [[probability]]
$$
P(\text{getting number of successes})=(\text{number of possible arragements})(\text{probability of success})^\text{number of successes}(\text{probability of failure})^\text{number of failures}
$$
$$
P(\text{exactly k successes})=_{n}C_{k}\cdot p^k\cdot(1-p)^k
$$
how many arrangements there are is equal to how many different ways there are of choosing k successes out of n trials, or $_{nC_{k}}$.

## [[expected value]] 
$$
E(X)=np
$$
We expect that we will get a success $p\%$ of the time, so we just take that percent of the number of trials to find the [[expected value]].

## [[variance]] 
let's first find the variance of a single trial of a binomial variable, where $1$ represents a success and $0$ a failure. The [[probability]] of a success is $p$, and the [[probability]] of a failure is $1-p$.

The [[expected value]] of binomial variable is $np$, or $1(p)=p$.  Another way of thinking about the [[expected value]] is by taking the weighted average of the outcomes. In this case, we have $(p)1+(1-p)0$, which is also $p$.

We know that for a [[random variable]],
![[random variable#^c893cd]]
Our only two possible values are 0 and 1
$$
\begin{align}
\text{Variance}=&p(1-E(x))^2+(1-p)(0-E(x))^2 \\
\text{Variance}=&p(1-p)^2+(1-p)(0-p)^2 \\
\text{Variance}=&p(1-p)^2+(1-p)(p)^2 \\
\text{Variance}=&p(1-p)((1-p)+(p)) &&\text{factor} \\
\text{Variance}=&p(1-p)
\end{align}
$$

^1eac37

![[random variable#^60a6fa]]
Thus, for each trial, we can add the [[variance]] for each trial. In other words, we multiply by the number of trials to find the total variance for the binomial [[distribution]].
> [!definition]
> $$
> \begin{align}
> \text{Variance}&=np(1-p) \\
> \text{Standard Deviation}&=\sqrt{ np(1-p) }
> \end{align}
> $$

