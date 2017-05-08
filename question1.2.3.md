# Solutions to Econometrics

by Qiang Gao, updated at Mar 21, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 2 The Algebra of Least Squares

...

#### Review Question 1.2.3 (OLS estimator for the simple regression model)

In the simple regression model, $$ K = 2 $$ and $$ x_{i1} = 1 $$. Show that

$$
\mathbf{S}_{\mathbf{x}\mathbf{x}} = 
\begin{bmatrix}
  1 & \bar{x}_2 \\
  \bar{x}_2 & \frac{1}{n} \sum_{i=1}^n x_{i2}^2
\end{bmatrix},
\quad
\mathbf{S}_{\mathbf{x}\mathbf{y}} =
\begin{bmatrix}
  \bar{y} \\ \frac{1}{n} \sum_{i=1}^n x_{i2} y_i
\end{bmatrix}
$$

where

$$
\bar{y} \equiv \frac{1}{n} \sum_{i=1}^n y_i,
\quad
\bar{x}_2 \equiv \frac{1}{n} \sum_{i=1}^n x_{i2}.
$$

Show that

$$
b_2 = \frac{ \frac{1}{n} \sum_{i=1}^n (x_{i2} - \bar{x}_2)(y_i - \bar{y}) }{ \frac{1}{n} \sum_{i=1}^n (x_{i2} - \bar{x}_2)^2 },
\quad
b_1 = \bar{y} - \bar{x}_2 b_2.
$$

##### Solution

(1)

$$
\begin{align}
  \mathbf{S}_{\mathbf{x}\mathbf{x}}
  & = \frac{1}{n} \mathbf{X}' \mathbf{X} \\
  & =
  \frac{1}{n}
  \begin{bmatrix}
    1 & \cdots & 1 \\
    x_{12} & \cdots & x_{n2}
  \end{bmatrix}
  \begin{bmatrix}
    1 & x_{12} \\
    \vdots & \vdots \\
    1 & x_{n2}
  \end{bmatrix} \\
  & =
  \frac{1}{n}
  \begin{bmatrix}
    n & \sum_{i=1}^n x_{i2} \\
    \sum_{i=1}^n x_{i2} & \sum_{i=1}^n x_{i2}^2
  \end{bmatrix} \\
  & =
  \begin{bmatrix}
  1 & \bar{x}_2 \\
  \bar{x}_2 & \frac{1}{n} \sum_{i=1}^n x_{i2}^2
  \end{bmatrix}
\end{align}
$$

(2)

$$
\begin{align}
  \mathbf{S}_{\mathbf{x}\mathbf{y}}
  & = \frac{1}{n} \mathbf{X}' \mathbf{y} \\
  & =
  \frac{1}{n}
  \begin{bmatrix}
    1 & \cdots & 1 \\
    x_{12} & \cdots & x_{n2}
  \end{bmatrix}
  \begin{bmatrix}
    y_1 \\
    \vdots \\
    y_n
  \end{bmatrix} \\
  & =
  \frac{1}{n}
  \begin{bmatrix}
    \sum_{i=1}^n y_i \\
    \sum_{i=1}^n x_{i2} y_i
  \end{bmatrix} \\
  & =
  \begin{bmatrix}
    \bar{y} \\
    \frac{1}{n} \sum_{i=1}^n x_{i2} y_i
  \end{bmatrix}
\end{align}
$$

(3) To solve for $$ \mathbf{b} $$ from

$$
\mathbf{S}_{\mathbf{x} \mathbf{x}}
\mathbf{b} =
\mathbf{S}_{\mathbf{x} \mathbf{y}},
$$

perform row operations on the following augmented matrix

$$
\begin{align}
  \begin{bmatrix}
    \mathbf{S}_{\mathbf{x} \mathbf{x}} |
    \mathbf{S}_{\mathbf{x} \mathbf{y}}
  \end{bmatrix}
  & =
  \begin{bmatrix}
    1 & \bar{x}_2 & \bar{y} \\
    \bar{x}_2 & \frac{1}{n} \sum_{i=1}^n x_{i2}^2
    & \frac{1}{n} \sum_{i=1}^n x_{i2} y_i
  \end{bmatrix} \\
  & \sim
  \begin{bmatrix}
    1 & \bar{x}_2 & \bar{y} \\
    0 & \frac{1}{n} \sum_{i=1}^n x_{i2}^2 - \bar{x}_2^2
    & \frac{1}{n} \sum_{i=1}^n x_{i2} y_i
    - \bar{x}_2 \bar{y}
  \end{bmatrix} \\
  & =
  \begin{bmatrix}
    1 & \bar{x}_2 & \bar{y} \\
    0 & \frac{1}{n} \sum_{i=1}^n (x_{i2} - \bar{x}_2)^2
    & \frac{1}{n} \sum_{i=1}^n 
    (x_{i2} - \bar{x}_2)(y_i - \bar{y})
  \end{bmatrix} \\
  & \sim
  \begin{bmatrix}
    1 & \bar{x}_2 & \bar{y} \\
    0 & 1 & 
    \frac{ \frac{1}{n} \sum_{i=1}^n
    (x_{i2} - \bar{x}_2)(y_i - \bar{y}) }
    {\frac{1}{n} \sum_{i=1}^n (x_{i2} - \bar{x}_2)^2}
  \end{bmatrix} \\
  & \sim
  \begin{bmatrix}
    1 & 0 & \bar{y} -
    \bar{x}_2
    \frac{ \frac{1}{n} \sum_{i=1}^n
    (x_{i2} - \bar{x}_2)(y_i - \bar{y}) }
    {\frac{1}{n} \sum_{i=1}^n (x_{i2} - \bar{x}_2)^2}
    \\
    0 & 1 &
    \frac{ \frac{1}{n} \sum_{i=1}^n
    (x_{i2} - \bar{x}_2)(y_i - \bar{y}) }
    {\frac{1}{n} \sum_{i=1}^n (x_{i2} - \bar{x}_2)^2}
  \end{bmatrix} \\
  & = 
  \begin{bmatrix}
    \mathbf{I} | \mathbf{b}
  \end{bmatrix}.
\end{align}
$$

So

$$
b_2 = \frac{ \frac{1}{n} \sum_{i=1}^n (x_{i2} - \bar{x}_2)(y_i - \bar{y}) }{ \frac{1}{n} \sum_{i=1}^n (x_{i2} - \bar{x}_2)^2 },
\quad
b_1 = \bar{y} - \bar{x}_2 b_2.
$$

##### Note

$$
b_2 \stackrel{p} \to \frac{\mathrm{Cov} (x_2, y)}{\mathrm{Var} (x_2)}
$$

---

Copyright ©2017 by Qiang Gao