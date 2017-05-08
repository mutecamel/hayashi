## Solutions to Review Question

by Qiang Gao, updated at May 8, 2017

---

#### Review Question 1.3.4 (Gauss-Markov for unconditional variance)

(a) Prove: $$ \mathrm{Var} ( \widehat{\boldsymbol{\beta}} ) = \mathrm{E} [  \mathrm{Var} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) ] + \mathrm{Var} [ \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) ] $$.

##### Solution

By the [formula of variance](supplements/var-matrix.md),

$$
\begin{align}
\mathrm{Var} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} )
& =
\mathrm{E} ( \widehat{\boldsymbol{\beta}} \widehat{\boldsymbol{\beta}}' | \mathbf{X} ) -
\mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} )
\mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} )'.
\end{align}
$$

Taking expectations,

$$
\begin{align}
\mathrm{E} [  \mathrm{Var} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) ]
& =
\mathrm{E} [ \mathrm{E} ( \widehat{\boldsymbol{\beta}} \widehat{\boldsymbol{\beta}}' | \mathbf{X} ) ] -
\mathrm{E} [ \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} )' ]
\\ & =
\mathrm{E} ( \widehat{\boldsymbol{\beta}} \widehat{\boldsymbol{\beta}}' ) -
\mathrm{E} [ \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} )' ].
\tag{1}
\end{align}
$$

Also by the [formula of variance](supplements/var-matrix.md),

$$
\begin{align}
\mathrm{Var} [ \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) ]
& =
\mathrm{E} [ \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} )' ] -
\mathrm{E} ( \widehat{ \boldsymbol{ \beta } } )
\mathrm{E} ( \widehat{ \boldsymbol{ \beta } } )'.
\tag{2}
\end{align}
$$

Combining equations (1) and (2), and again by the [formula of variance](supplements/var-matrix.md),

$$
\mathrm{E} [  \mathrm{Var} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) ] +
\mathrm{Var} [ \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) ]
=
\mathrm{E} ( \widehat{\boldsymbol{\beta}} \widehat{\boldsymbol{\beta}}' ) -
\mathrm{E} ( \widehat{ \boldsymbol{ \beta } } )
\mathrm{E} ( \widehat{ \boldsymbol{ \beta } } )'
=
\mathrm{Var} ( \widehat{ \boldsymbol{ \beta } } ).
$$

(b) Prove (1.3.3) in textbook,

$$
\mathrm{Var} ( \widehat{ \boldsymbol{ \beta } } ) \ge
\mathrm{Var} ( \mathbf{b} ),
\tag{1.3.3}
$$

where $$ \widehat{ \boldsymbol{ \beta } } $$ is any linear unbiased estimator.

##### Solution

$$
\begin{align}
& \mathrm{Var} ( \widehat{ \boldsymbol{ \beta } } ) -
\mathrm{Var} ( \mathbf{b} )
\\ = &
\mathrm{E} [  \mathrm{Var} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) ] + \mathrm{Var} [ \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) ] -
\mathrm{E} [ \mathrm{Var} ( \mathbf{b} | \mathbf{X} ) ] - \mathrm{Var} [ \mathrm{E} ( \mathbf{b} | \mathbf{X} ) ]
\\ &
\text{(by part (a))}
\\ = &
\mathrm{E} [  \mathrm{Var} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) ] -
\mathrm{E} [ \mathrm{Var} ( \mathbf{b} | \mathbf{X} ) ]
\qquad
\text{($ \mathrm{E} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) = \mathrm{E} ( \mathbf{b} | \mathbf{X} ) = \boldsymbol{ \beta } $)}
\\ = &
\mathrm{E} [  \mathrm{Var} ( \widehat{\boldsymbol{\beta}} | \mathbf{X} ) - \mathrm{Var} ( \mathbf{b} | \mathbf{X} ) ]
\qquad \text{(linearity of expectations)}
\\ = &
\text{postive semidefinite matrix}.
\qquad \text{(Gauss-Markov Theorem)}
\end{align}
$$

---

Copyright ©2017 by Qiang Gao