+ trial outcomes are either successes or failures
+ trials are [[independent]] 
+ same [[probability]] on each trial
+ unknown number of trials
> [!example]
> + How many trials until success?
> + Number of rolls until we get a 6

the [[probability distribution]] of a geometric variable is a geometric [[distribution]]. This [[distribution]] is right skewed, as theoretically your numbers of trials could approach [[infinity]], but they are much more likely to occur sooner than that.

## [[mean]] 
$X$ is the number of trials to get our success. p is the [[probability]] of a success.

$$
\begin{align}
\mu_{X}&=P(X=1)\cdot1+P(X=2)\cdot2+P(X-3)\cdot3+\dots &&\text{expected value is the weighted average of possible outcomes}\\
\mu_{X}&=p\cdot1+(1-p)(p)\cdot2+(1-p)^2p\cdot3+\dots&&\text{the probability of each outcome is equal to p times how many failures before} \\
\mu_{X}=1p+&2p(1-p)+3p(1-p)^2p+\dots &&\text{simplify}\\
(1-p)\mu_{X}=&1p(1-p)+2p(1-p)^2+3p(1-p)^3+\dots \\
\mu_{X}-(1-p)\mu_{X}=1p+&1p(1-p)+1p(1-p)^2+\dots &&\text{subtract straight down }\\
\mu_{X}+(p-1)\mu_{X}=& \\
\mu_{X}+\mu_{X}\cdot p-\mu _{X} =&\\
p\cdot \mu _{X}=1p+&1p(1-p)+1p(1-p)^2+\dots & \\
\mu _{X}=1+&(1-p)+(1-p)^2\dots &&\text{divide both sides by p, this is a geometric series} \\
-(1-p)\mu_{X}=-&(1-p)-(1-p)^2-\dots \\
\mu_{X}-(1-p)\mu_{X}=1-&(1-p)^n &&\text{subtract down}\\
\mu_{X}(1-(1-p))=1-(1-p)^n \\
\mu_{X}(1-1+p)=1&(1-p)^n &&\text{approaches 0 and becomes negligible as n approaches infinity}  \\
\mu_{X}=\frac{1}{p}
\end{align}
$$


$$\mu _{x}=\frac{1}{p}$$
> [!example]
> The odds of getting a 6 on a die is $\frac{1}{6}$. Thus, it would take on average 6 tries to roll a 6.
> 
## [[standard deviation]] 
$$
\sigma_{X}=\frac{\sqrt{ 1-p }}{p}
$$

