# Solutions to Econometrics

by Qiang Gao, updated at May 8, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 3 Finite-Sample Properties of OLS

...

#### Review Question 1.3.6

Prove part (d) of Proposition 1.1, under Assumptions 1.1—1.4, $$ \mathrm{Cov} ( \mathbf{b}, \mathbf{e} | \mathbf{X} ) = \mathbf{0} $$, where $$ \mathbf{e} \equiv \mathbf{y} - \mathbf{X} \mathbf{b} $$.

##### Solution

By definition,

$$
\begin{align}
\mathrm{Cov} ( \mathbf{b}, \mathbf{e} | \mathbf{X} )
& =
\mathrm{E} \{ [ \mathbf{b} - \mathrm{E} ( \mathbf{b} | \mathbf{X} ) ][ \mathbf{e} - \mathrm{E} ( \mathbf{e} | \mathbf{X} ) ]' | \mathbf{X} \}
\\ & =
\mathrm{E} \{ [ \mathbf{A} \boldsymbol{ \varepsilon } ][ \mathbf{M} \boldsymbol{ \varepsilon } ]' | \mathbf{X} \}
\qquad \text{ ($ \mathbf{A} \equiv (\mathbf{X}' \mathbf{X})^{-1} \mathbf{X}' $, $ \mathbf{M} \equiv \mathbf{I} - \mathbf{X}
( \mathbf{X}' \mathbf{X} )^{-1} \mathbf{X}' $) }
\\ & =
\mathbf{A} \mathrm{E} ( \boldsymbol{ \varepsilon } \boldsymbol{\varepsilon}' | \mathbf{X} ) \mathbf{M}'
\\ & =
\sigma^2 \mathbf{A} \mathbf{M}'.
\end{align}
$$

---

Copyright ©2017 by Qiang Gao