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
\mathrm{E} ( \mathbf{x} )' \mathbf{x} +
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

---

Copyright ©2017 by Qiang Gao