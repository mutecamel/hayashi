# Solution to Review Question

by Qiang Gao, updated at Mar 13, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 1 The Classical Linear Regression Model

...

#### Review Question 1.1.6 (An exercise in conditional and unconditional expectations)

Show that Assumptions 1.2 and 1.4 imply

$$
\begin{align}
  \mathrm{Var} ( \varepsilon_i )
  & = \sigma^2
  \qquad
  (i = 1, 2, \ldots, n) \\
  \text{and}
  \qquad
  \mathrm{Cov} ( \varepsilon_i, \varepsilon_j ) & = 0
  \qquad
  (i \neq j; i, j = 1, 2, \ldots, n).  \tag{$\ast$}
\end{align}
$$

##### Solution

Strict exogeneity implies $$ \mathrm{E} (\varepsilon_i) = 0 $$. So $$ (\ast) $$ is equivalent to

$$
\begin{align}
  \mathrm{E} ( \varepsilon_i^2 ) & = \sigma^2
  \qquad
  (i = 1, 2, \ldots, n) \\
  \text{and}
  \qquad
  \mathrm{E} ( \varepsilon_i \varepsilon_j ) & = 0
  \qquad
  (i \neq j; i, j = 1, 2, \ldots, n).
\end{align}
$$

(1) For $$i = 1, 2, \ldots, n$$,

$$
\begin{align}
  \mathrm{E} (\varepsilon_i^2)
  & =
  \mathrm{E} [\mathrm{E} (\varepsilon_i^2 | \mathbf{X})]
  \qquad
  \text{(law of total expectations)}
  \\
  
  & =
  \sigma^2. \qquad \text{(Assumption 1.4)}
\end{align}
$$

(2) For $$i \neq j; i, j = 1, 2, \ldots, n$$,

$$
\begin{align}
  \mathrm{E} (\varepsilon_i \varepsilon_j)
  & =
  \mathrm{E} [
  \mathrm{E} (\varepsilon_i \varepsilon_j | \mathbf{X})
  ]
  \qquad
  \text{(law of total expectations)}
  \\
  
  & =
  0. \qquad \text{(Assumption 1.4)}
\end{align}
$$

---

Copyright ©2017 by Qiang Gao