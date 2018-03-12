## Matrix Multiplication Rules

by Qiang Gao, updated at Mar 20, 2017

---

Matrix multiplication can be defined equivalently in _four_ different ways as following, where vector $$ \mathbf{a} $$ is  _column_ vector by default and $$ \mathbf{a}^\intercal $$ means corresponding _row_ vector, the transpose of $$ \mathbf{a} $$.

#### Definition (inner-way multiplication)

$$
\begin{align}
  \mathbf{A}_{m \times n} \mathbf{B}_{n \times p}
  & = 
  \begin{bmatrix}
    — & \boldsymbol{\alpha}_1^\intercal & — \\
      & \vdots & \\
    — & \boldsymbol{\alpha}_m^\intercal & —
  \end{bmatrix}
  \begin{bmatrix}
    | & & | \\
    \mathbf{b}_1 & \cdots & \mathbf{b}_p \\
    | & & |
  \end{bmatrix} \\
  & =
  \begin{bmatrix}
    \boldsymbol{\alpha}_1^\intercal \mathbf{b}_1
      & \cdots
      & \boldsymbol{\alpha}_1^\intercal \mathbf{b}_p \\
    \vdots & \ddots & \vdots \\
    \boldsymbol{\alpha}_m^\intercal \mathbf{b}_1
      & \cdots
      & \boldsymbol{\alpha}_m^\intercal \mathbf{b}_p
  \end{bmatrix}
\end{align}
$$

#### Definition (outer-way multiplication)

$$
\begin{align}
  \mathbf{A}_{m \times n} \mathbf{B}_{n \times p}
  & =
  \begin{bmatrix}
    | & & | \\
    \mathbf{a}_1 & \cdots & \mathbf{a}_n \\
    | & & |
  \end{bmatrix}
  \begin{bmatrix}
    — & \boldsymbol{\beta}_1^\intercal & — \\
    & \vdots & \\
    — & \boldsymbol{\beta}_n^\intercal & —
  \end{bmatrix} \\
  & =
  \sum_{i=1}^n \mathbf{a}_i \boldsymbol{\beta}_i^\intercal
\end{align}
$$

#### Definition (column-way multiplication)

$$
\begin{align}
  \mathbf{A}_{m \times n} \mathbf{B}_{n \times p}
  & =
  \begin{bmatrix}
    | & & | \\
    \mathbf{a}_1 & \cdots & \mathbf{a}_n \\
    | & & |
  \end{bmatrix}
  \begin{bmatrix}
    | & & | \\
    \mathbf{b}_1 & \cdots & \mathbf{b}_p \\
    | & & |
  \end{bmatrix} \\
  & =
  \begin{bmatrix}
    | & & | \\
    \sum_{i=1}^n b_{i1} \mathbf{a}_i
      & \cdots
      & \sum_{i=1}^n
      b_{ip} \mathbf{a}_i \\
    | & & |
  \end{bmatrix}
\end{align}
$$

#### Definition (row-way multiplication)

$$
\begin{align}
  \mathbf{A}_{m \times n} \mathbf{B}_{n \times p}
  & =
  \begin{bmatrix}
    — & \boldsymbol{\alpha}_1^\intercal & — \\
    & \vdots & \\
    — & \boldsymbol{\alpha}_m^\intercal & —
  \end{bmatrix}
  \begin{bmatrix}
    — & \boldsymbol{\beta}_1^\intercal & — \\
    & \vdots & \\
    — & \boldsymbol{\beta}_n^\intercal & —
  \end{bmatrix} \\
  & =
  \begin{bmatrix}
    — & \sum_{i=1}^n a_{1i}
      \boldsymbol{\beta}_i^\intercal & — \\
    & \vdots & \\
    — & \sum_{i=1}^n a_{mi}
      \boldsymbol{\beta}_i^\intercal & —
  \end{bmatrix}
\end{align}
$$

##### Note

- If you are concerning _each element_ of the result of $$ \mathbf{A} \mathbf{B} $$, then you should use the inner-way multiplication.

- If you want the express $$ \mathbf{A} \mathbf{B} $$ as a _sum_, then you should use the outer-way multiplication.

- If you are concerning _each column_ of the result of $$ \mathbf{A} \mathbf{B} $$, then you should use the column-way multiplication.

- If you are concerning _each row_ of the result of $$ \mathbf{A} \mathbf{B} $$, then you should use the row-way multiplication.

---

Copyright ©2018 by Qiang Gao