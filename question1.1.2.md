# Solutions to Econometrics

by Qiang Gao, updated at Mar 20, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 1 The Classical Linear Regression Model

...

#### Review Question 1.1.2 (Conditional cross-moment of error terms)

Prove the last equality in (1.1.15),

$$
\mathrm{E} (\varepsilon_i \varepsilon_j | \mathbf{X})
=
\mathrm{E} (\varepsilon_i | \mathbf{x}_i)
\mathrm{E} (\varepsilon_j | \mathbf{x}_j)
\qquad
\text{(for $i \neq j$)}.
\tag{1.1.15}
$$

##### Solution
$$
\begin{align}
  \mathrm{E} ( \varepsilon_i \varepsilon_j | \mathbf{X} )
  & = \mathrm{E} [ \mathrm{E} ( \varepsilon_i \varepsilon_j | \mathbf{X}, \varepsilon_j ) | \mathbf{X} ]
  \qquad
  \text{(law of iterated expectations)}
  \\ 
  & = \mathrm{E} [ \varepsilon_j \mathrm{E} ( \varepsilon_i | \mathbf{X}, \varepsilon_j ) | \mathbf{X} ]
  \qquad
  \text{($\varepsilon_j$ is constant under condition)}
  \\
  & = \mathrm{E} [ \varepsilon_j \mathrm{E} ( \varepsilon_i | \mathbf{x}_i ) | \mathbf{X} ]
  \qquad
  \text{(random sample)} \\
  & = \mathrm{E} ( \varepsilon_i | \mathbf{x}_i ) \mathrm{E} ( \varepsilon_j | \mathbf{X})
  \qquad
  \text{($\mathbf{x}_i$ is known conditional on $\mathbf{X}$)} \\
  & = \mathrm{E} ( \varepsilon_i | \mathbf{x}_i ) \mathrm{E} ( \varepsilon_j | \mathbf{x}_j)
  \qquad
  \text{(random sample)}
\end{align}
$$

---

Copyright ©2017 by Qiang Gao