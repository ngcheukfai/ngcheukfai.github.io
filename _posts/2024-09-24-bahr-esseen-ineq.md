---
title: 'Bahr and Esseen Inequality'
date: 2024-09-24
permalink: /posts/2024/08/bahr-esseen/
tags:
  - Statistics
---

Bahr and Esseen (1965) Inequality provides a useful moment bound on the absolute sum of independent variable. It states as follows: let $$X_1,X_2,\ldots , X_n$$ be a sequence of independent r.v.'s with $$EX_i=0$$ and $E|X_i|<\infty,1\leq i\leq n.$ If $$r$$ satisfies 
$$
\begin{aligned}
D(r)=\frac{13.52}{(2.6 \pi)^r}\Gamma(r)\sin (r\pi/2)<1 \text{ and } 1\leq r \leq 2,
\end{aligned}
$$
then $$E|\sum^n_{i=1}X_i|^r\leq \frac{1}{1-D(r)}\sum^n_{i=1}|X_i|^r.
$$
	
<img src='/images/D_function.png'>

##### Reference

*Von Bahr, B. E. N. G. T., and Carl-Gustav Esseen. "Inequalities for the rth absolute moment of a sum of random variables, $$1\leq r\leq 2$$." The Annals of Mathematical Statistics (1965): 299-303.*