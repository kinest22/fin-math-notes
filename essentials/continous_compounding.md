## Discrete compounded vs continuous compounded interest rates 
In practical use, one can often find rates being used in a discrete setting whereas academics and model developers tend to prefer continuous time setting. The former is closer to the real life (where bond coupons, for instance, occur every 6 months). The latter is more convienient. Exponential functions are easy to deal with, easy to differentiate and multiply. The richness of the theory of continuous time processes often allows one to obtain analytical results that would be unavailable in discrete time.

It should be pointed out that there is no any rationale to use continuously compounded interest rates instead of discrete ones. As long as both formulae are applied correctly, same (correct) results will always be obtained. 

## Idea of interest compounding
The idea of interest compounding could be formalized using accumulation function $a(t,n)$ that shows how many times the initial amount $P_0$ will increase after t years:
$$a(\tau, m)=\left( 1+\frac{r}{m} \right)^{m\tau}$$ where:
$\tau$ - overall length of time the interest is applied (in years),
$m$ - compounding frequency,
$r$ - annual interest rate.

For a special case when compounding occures once per year ($m=1$):
$$a(\tau, 1)=\left( 1+r \right)^{\tau}=(1+r)(1+r)(1+r)...$$ 

From definition of $a(\tau,m)$ above it follows that the effective interest rate that takes interest compoinding into account is:

$$R_m(\tau)=a(\tau, m)-1$$

And total accumulated value in $\tau$ years could be obtained as follows:

$$
\begin{split}
P(\tau,m)&=P_0(1+R_m(\tau))\\
&=P_0a(\tau, m)\\
&=P_0\left( 1+\frac{r}{m} \right)^{m\tau}
\end{split}
$$

## From discrete to continuous compounding
When the number of compounding periods per year increases without limit, continuous compounding occurs. Continuous compounding can be regarded as letting the compounding period become infinitesimally small. This can be achieved by taking the limit of $a(\tau, m)$ as $m$ goes to infinity: 
$$
\begin{align}
\lim_{m\to\infty} a(\tau, m) &= \lim_{m\to\infty} \left( 1+\frac{r}{m} \right)^{m\tau} \\
&=\left[ \lim_{m\to\infty} \left( 1+\frac{r}{m} \right)^{\frac{m}{r}} \right]^{m\tau \frac{r}{m}} \\
&=e^{r\tau}
\end{align}
$$

>##### Note on transformation (2) $\to$ (3)
>Recalling from calculus that:
$$\lim_{x\to\infty}\left(1+\frac{1}{x} \right)^{x}=e$$ we can introduce variable change $\rho=\frac{m}{r}$ such that:
$$\left[ \lim_{m\to\infty} \left( 1+\frac{r}{m} \right)^{\frac{m}{r}} \right]^{m\tau \frac{r}{m}}=\left[ \lim_{\rho\to\infty} \left( 1+\frac{1}{\rho} \right)^{\rho} \right]^{r\tau}=e^{r\tau}$$ 

The amount $P(\tau)$ after $\tau$ periods of continuous compounding can now be expressed in terms of the initial amount $P_0$ as:
$$P(\tau) =P_0e^{r\tau}$$ which implies that accumulation function in terms of continuous compounding has the form of:
$$a(\tau)=e^{r\tau}$$ Hence the effective interest rate in continuous compounding setting could be defined as:
$$R(\tau)=a(\tau)-1=e^{r\tau}-1$$
