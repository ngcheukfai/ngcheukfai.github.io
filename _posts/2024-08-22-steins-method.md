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
Typically, the function $h$ would be the indicator function $$h(w)=I(w\leq z)$$ and $$Z$$ is normal. So it becomes
$$
\begin{aligned}
f'(w)-wf(w)=I(w\leq z)-\Phi(z).
\end{aligned}
$$

Let $$Z$$ be a standard normally distrbuted random variable and let $$\mathscr{C}$$ be the set of continuous and piecewise continuously differentiable functions $$f:\mathbb{R}\rightarrow \mathbb{R}$$ with $$E\lvert f'(Z)\rvert<\infty$$.

##### Reference

*Normal Approximation by Stein’s Method (Probability and Its Applications), Louis H.Y. Chen, Larry Goldstein, Qi-Man Shao.*