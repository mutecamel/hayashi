# Solutions to Econometrics

by Qiang Gao, updated at Mar 21, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 2 The Algebra of Least Squares

...

#### Review Question 1.2.4

Prove that

$$
\begin{gather}
  \text{
    Both $ \mathbf{P} $ and $ \mathbf{M} $ are symmetric and idempotent,
  } \tag{1.2.9} \\
  \mathbf{P} \mathbf{X} = \mathbf{X} \quad
  \text{(hence the term projection matrix),}\tag{1.2.10}\\
  \mathbf{M} \mathbf{X} = \mathbf{0} \quad
  \text{(hence the term annihilator).}\tag{1.2.11}
\end{gather}
$$

##### Solution

(1) $$ \mathbf{P} $$ is symmetric because

$$
\begin{align}
  \mathbf{P}^\intercal 
  & =
  [\mathbf{X} (\mathbf{X}^\intercal \mathbf{X})^{-1}
  \mathbf{X}^\intercal]^\intercal
  \qquad
  \text{(definition (1.2.7))}
  \\
  & =
  (\mathbf{X}^\intercal)^\intercal
  [(\mathbf{X}^\intercal \mathbf{X})^{-1}]^\intercal
  \mathbf{X}^\intercal
  \qquad
  ((\mathbf{A} \mathbf{B}^\intercal) = 
  \mathbf{B}^\intercal \mathbf{A}^\intercal)
  \\
  & = 
  (
  \mathbf{X}^\intercal)^\intercal
  [(\mathbf{X}^\intercal \mathbf{X})^\intercal]^{-1}
  \mathbf{X}^\intercal
  \qquad
  ((\mathbf{A}^{-1})^\intercal =
  (\mathbf{A}^\intercal)^{-1})
  \\
  & =
  \mathbf{X} (\mathbf{X}^\intercal \mathbf{X})^{-1}
  \mathbf{X}^\intercal
  \qquad
  ((\mathbf{A}^\intercal)^\intercal = \mathbf{A})
  \\
  & =
  \mathbf{P}.
  \qquad
  \text{(definition (1.2.7))}
\end{align}
$$

(2) $$ \mathbf{M} $$ is symmetric because

$$
\begin{align}
  \mathbf{M}^\intercal
  & =
  ( \mathbf{I} - \mathbf{P} )^\intercal
  \qquad
  \text{(definition (1.2.8))}
  \\
  & =
  \mathbf{I}^\intercal - \mathbf{P}^\intercal
  \qquad
  ((\mathbf{A} - \mathbf{B})^\intercal =
  \mathbf{A}^\intercal - \mathbf{B}^\intercal)
  \\
  & =
  \mathbf{I} - \mathbf{P}
  \qquad
  \text{($\mathbf{I}$ and $\mathbf{P}$ are symmetric)}
  \\
  & =
  \mathbf{M}.
  \qquad
  \text{(definition (1.2.8))}
\end{align}
$$

(3) $$ \mathbf{P} $$ is idempotent because

$$
\begin{align}
  \mathbf{P}^2 & =
  (\mathbf{X} (\mathbf{X}^\intercal \mathbf{X})^{-1}
  \mathbf{X}^\intercal) \cdot (\mathbf{X}
  (\mathbf{X}^\intercal \mathbf{X})^{-1}
  \mathbf{X}^\intercal)
  \qquad
  \text{(definition (1.2.7))}
  \\
  & =
  \mathbf{X} (\mathbf{X}^\intercal \mathbf{X})^{-1}
  (\mathbf{X}^\intercal \mathbf{X})
  (\mathbf{X}^\intercal \mathbf{X})^{-1}
  \mathbf{X}^\intercal
  \qquad
  ((\mathbf{A} \mathbf{B}) \mathbf{C} =
  \mathbf{A} (\mathbf{B} \mathbf{C}))
  \\
  & =
  \mathbf{X} (\mathbf{X}^\intercal \mathbf{X})^{-1}
  \mathbf{X}^\intercal
  \qquad
  (\mathbf{A}^{-1} \mathbf{A} = \mathbf{I})
  \\
  & = 
  \mathbf{P}.
  \qquad
  \text{(definition (1.2.7))}
\end{align}
$$

(4) $$ \mathbf{M} $$ is idempotent because

$$
\begin{align}
  \mathbf{M}^2 & = 
  (\mathbf{I} - \mathbf{P})(\mathbf{I} - \mathbf{P})
  \qquad
  \text{(definition (1.2.8))}
  \\
  & =
  \mathbf{I} - \mathbf{P} - \mathbf{P} + \mathbf{P}^2
  \\
  & =
  \mathbf{I} - \mathbf{P} - \mathbf{P} + \mathbf{P}
  \qquad
  \text{($\mathbf{P}$ is idempotent)}
  \\
  & =
  \mathbf{I} - \mathbf{P}
  \\
  & =
  \mathbf{M}.
  \qquad
  \text{(definition (1.2.8))}
\end{align}
$$

(5) $$ \mathbf{P} \mathbf{X} = \mathbf{X} $$ because

$$
\begin{align}
  \mathbf{P} \mathbf{X} 
  & = 
  \mathbf{X} (\mathbf{X}^\intercal \mathbf{X})^{-1}
  \mathbf{X}^\intercal \cdot \mathbf{X}
  \qquad
  \text{(definition (1.2.7))}
  \\
  & =
  \mathbf{X} (\mathbf{X}^\intercal \mathbf{X})^{-1}
  (\mathbf{X}^\intercal \mathbf{X})
  \\
  & =
  \mathbf{X}.
\end{align}
$$

(6) $$ \mathbf{M} \mathbf{X} = \mathbf{0} $$ because

$$
\begin{align}
  \mathbf{M} \mathbf{X} 
  & =
  ( \mathbf{I} - \mathbf{P} ) \mathbf{X}
  \qquad
  \text{(definition (1.2.8))}
  \\
  & =
  \mathbf{X} - \mathbf{P} \mathbf{X}
  \\
  & =
  \mathbf{X} - \mathbf{X}
  \qquad
  ( \mathbf{P} \mathbf{X} = \mathbf{X} )
  \\
  & =
  \mathbf{0}.
\end{align}
$$

---

Copyright ©2017 by Qiang Gao