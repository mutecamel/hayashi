# Solutions to Econometrics

by Qiang Gao, updated at May 8, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 3 Finite-Sample Properties of OLS

...

#### Review Question 1.3.7

Prove (1.2.21),

$$
0 \le p_i \le 1 \text{ and } \sum_{i=1}^{n} p_i = K,
\tag{1.2.21}
$$

where 

$$
p_i \equiv \mathbf{x}_i' ( \mathbf{X}' \mathbf{X} )^{-1} \mathbf{x}_i.
\tag{1.2.20}
$$

##### Solution

Because

$$
\mathbf{P} \equiv \mathbf{X} ( \mathbf{X}' \mathbf{X} )^{-1} \mathbf{ X }',
$$

$$ p_i $$ is the $$i$$-th row and $$i$$-th column of $$ \mathbf{P} $$. Because $$ \mathbf{P} $$ is positive semidefinite, $$ p_i \ge 0 $$. Similarly, because

$$
\mathbf{M} \equiv \mathbf{I} - \mathbf{X} ( \mathbf{X}' \mathbf{X} )^{-1} \mathbf{ X }',
$$

$$ 1 - p_i $$ is the $$i$$-th row and $$i$$-th column of $$ \mathbf{M} $$. Because $$ \mathbf{M} $$ is positive semidefinite, $$ 1 - p_i \ge 0 $$, $$ p_i \le 1 $$.

Finally,

$$
\begin{align}
\sum_{i=1}^n p_i 
& =
\mathrm{trace} ( \mathbf{P} )
\\ & =
\mathrm{trace} ( \mathbf{X} ( \mathbf{X}' \mathbf{X} )^{-1} \mathbf{ X }' )
\\ & =
\mathrm{trace} ( ( \mathbf{X}' \mathbf{X} )^{-1} \mathbf{ X }' \mathbf{X} )
\\ & =
\mathrm{trace} ( \mathbf{I}_K )
\\ & =
K.
\end{align}
$$

---

Copyright ©2017 by Qiang Gao