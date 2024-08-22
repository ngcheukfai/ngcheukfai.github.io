---
title: 'Stein&apos;s Method'
date: 2024-08-22
permalink: /posts/2024/08/steins-method/
tags:
  - Statistics
---

Stein's method is a way to show that a random variable $$W$$ has a distribution that is close to a target distribution (usually the normal distribution). Its idea is that if two random variables are similar, then the expectations of some functions of the two random variables being compared should be similar.

The central idea rests on the so called Stein&apos;s equation
$$
\begin{aligned}
f'(w)-wf(w)=h(w)-Eh(Z).
\end{aligned}
$$
Typically, the function $$h$$ would be the indicator function $$h(w)=I(w\leq z)$$ and $$Z$$ is normal. So it becomes
$$
\begin{aligned}
f'(w)-wf(w)=I(w\leq z)-\Phi(z).
\end{aligned}
$$
The above is a differential equation and has a solution $$f_z(\cdot)$$. The functions are measurable so we can plug back in the random variable $$W$$ (a bit informal). We can take expectation and obtain
$$
\begin{aligned}
E\Big(f_z'(W)-wf_z(W)\Big)=P(W\leq z)-\Phi(z).
\end{aligned}
$$
Then our job is to show that $$E\Big(f_z'(W)-wf_z(W)\Big)\rightarrow 0$$ which would imply $$P(W\leq z)-\Phi(z)\rightarrow 0$$.

##### Reference

*Normal Approximation by Stein’s Method (Probability and Its Applications), Louis H.Y. Chen, Larry Goldstein, Qi-Man Shao.*