# Solutions to Econometrics

by Qiang Gao, updated at Mar 21, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 2 The Algebra of Least Squares

...

#### Review Question 1.2.5 (Matrix algebra of fitted values and residuals)

Show the following:

(a) $$ \hat{\mathbf{y}} = \mathbf{P} \mathbf{y} $$, $$ \mathbf{e} = \mathbf{M} \mathbf{y} = \mathbf{M} \boldsymbol{\varepsilon} $$.

(b) $$ \mathrm{SSR} = \boldsymbol{\varepsilon}' \mathbf{M} \boldsymbol{\varepsilon} $$.

##### Solution

(a.1) $$ \hat{\mathbf{y}} = \mathbf{P} \mathbf{y} $$ because

$$
\begin{align}
  \hat{\mathbf{y}} & =
  \mathbf{X} \mathbf{b}
  \qquad
  \text{(definition of $\hat{\mathbf{y}}$)}
  \\
  & =
  \mathbf{X} ( \mathbf{X}' \mathbf{X} )^{-1} \mathbf{X}'
  \mathbf{y}
  \qquad
  \text{(definition of $\mathbf{b}$)}
  \\
  & =
  \mathbf{P} \mathbf{y}.
  \qquad
  \text{(definition of $\mathbf{P}$)}
\end{align}
$$

(a.2) $$ \mathbf{e} = \mathbf{M} \mathbf{y} = \mathbf{M} \boldsymbol{\varepsilon} $$ because

$$
\begin{align}
  \mathbf{e} & = \mathbf{y} - \mathbf{X} \mathbf{b}
  \qquad
  \text{(definition of $\mathbf{e}$)}
  \\
  & =
  \mathbf{y} - \hat{\mathbf{y}}
  \qquad
  \text{(definition of $\hat{\mathbf{y}}$)}
  \\
  & =
  \mathbf{y} - \mathbf{P} \mathbf{y}
  \qquad
  (\hat{\mathbf{y}} = \mathbf{P} \mathbf{y})
  \\
  & =
  (\mathbf{I} - \mathbf{P}) \mathbf{y}
  \\
  & =
  \mathbf{M} \mathbf{y}
  \qquad
  \text{(definition of $\mathbf{M}$)}
  \\
  & =
  \mathbf{M} ( \mathbf{X} \boldsymbol{\beta} + 
  \boldsymbol{\varepsilon} )
  \qquad
  \text{(Assumption 1.1)}
  \\
  & =
  \mathbf{M} \mathbf{X} \boldsymbol{\beta} +
  \mathbf{M} \boldsymbol{\varepsilon}
  \\
  & =
  \mathbf{M} \boldsymbol{\varepsilon}
  \qquad
  (\mathbf{M} \mathbf{X} = \mathbf{0})
\end{align}
$$

(b) $$ \mathrm{SSR} = \boldsymbol{\varepsilon}' \mathbf{M} \boldsymbol{\varepsilon} $$ because

$$
\begin{align}
  \mathrm{SSR} & = \mathbf{e}' \mathbf{e}
  \qquad
  \text{(definition of $\mathrm{SSR}$)}
  \\
  & =
  (\mathbf{M} \boldsymbol{\varepsilon})'
  (\mathbf{M} \boldsymbol{\varepsilon})
  \qquad
  ( \mathbf{e} = \mathbf{M} \boldsymbol{\varepsilon} )
  \\
  & =
  \boldsymbol{\varepsilon}' \mathbf{M} \mathbf{M}
  \boldsymbol{\varepsilon}
  \\
  & =
  \boldsymbol{\varepsilon}' \mathbf{M}
  \boldsymbol{\varepsilon}.
  \qquad
  \text{($\mathbf{M}$ is idempotent)}
\end{align}
$$

---

Copyright ©2017 by Qiang Gao