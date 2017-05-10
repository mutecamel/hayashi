# Variance-Covariance Matrix of Random Vectors

by Qiang Gao, updated at May 8, 2017

---

The **variance-covariance matrix** of a random vector $$ \mathbf{x} $$ is defined as

$$
\begin{align}
\mathrm{Var} ( \mathbf{x} ) & \equiv
\mathrm{E} [ ( \mathbf{x} - \mathrm{E} ( \mathbf{x} ) )
( \mathbf{x} - \mathrm{E} ( \mathbf{x} ) )' ]
\qquad \text{(the definition)}
\\ & =
\mathrm{E} [ \mathbf{x} \mathbf{x}' -
\mathbf{x} \mathrm{E} ( \mathbf{x} )' -
\mathrm{E} ( \mathbf{x} ) \mathbf{x}' +
\mathrm{E} ( \mathbf{x} ) \mathrm{E} ( \mathbf{x} )' ]
\\ & =
\mathrm{E} ( \mathbf{x} \mathbf{x}' ) -
\mathrm{E} ( \mathbf{x} ) \mathrm{E} ( \mathbf{x} )' -
\mathrm{E} ( \mathbf{x} ) \mathrm{E} ( \mathbf{x} )' +
\mathrm{E} ( \mathbf{x} ) \mathrm{E} ( \mathbf{x} )'
\\ & =
\mathrm{E} ( \mathbf{x} \mathbf{x}' ) -
\mathrm{E} ( \mathbf{x} ) \mathrm{E} ( \mathbf{x} )'.
\qquad \text{(the formula)}
\end{align}
$$

The last equation is the convenient formula for calculating variance.

The **covariance matrix** between two random vectors $$ \mathbf{x} $$ and $$ \mathbf{y} $$ is defined as

$$
\begin{align}
\mathrm{Cov} ( \mathbf{x}, \mathbf{y} ) & \equiv
\mathrm{E} [ ( \mathbf{x} - \mathrm{E} ( \mathbf{x} ) )
( \mathbf{y} - \mathrm{E} ( \mathbf{y} ) )' ]
\qquad \text{(the definition)}
\\ & =
\mathrm{E} [ \mathbf{x} \mathbf{y}' -
\mathbf{x} \mathrm{E} ( \mathbf{y} )' -
\mathrm{E} ( \mathbf{x} ) \mathbf{y}' +
\mathrm{E} ( \mathbf{x} ) \mathrm{E} ( \mathbf{y} )' ]
\\ & =
\mathrm{E} ( \mathbf{x} \mathbf{y}' ) -
\mathrm{E} ( \mathbf{x} ) \mathrm{E} ( \mathbf{y} )' -
\mathrm{E} ( \mathbf{x} ) \mathrm{E} ( \mathbf{y} )' +
\mathrm{E} ( \mathbf{x} ) \mathrm{E} ( \mathbf{y} )'
\\ & =
\mathrm{E} ( \mathbf{x} \mathbf{x}' ) -
\mathrm{E} ( \mathbf{x} ) \mathrm{E} ( \mathbf{x} )'.
\qquad \text{(the formula)}
\end{align}
$$

The last equation is the convenient formula for calculating variance.

---

Copyright ©2017 by Qiang Gao