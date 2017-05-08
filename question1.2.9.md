# Solutions to Econometrics

by Qiang Gao, updated at Mar 26, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 2 The Algebra of Least Squares

...

#### Review Question 1.2.9 (Computation of the statistics)

Verify that $$ \mathbf{b} $$, $$ \mathrm{SSR} $$, $$ s^2 $$, and $$ R^2 $$ can be calculated from the following sample averages: $$ \mathbf{S}_{ \mathbf{x} \mathbf{x} } $$, $$ \mathbf{s}_{ \mathbf{x} \mathbf{y} } $$, $$ \mathbf{y}' \mathbf{y} / n $$, and $$ \bar{y} $$. (If the regressors include a constant, then $$ \bar{y} $$ is the element of $$ \mathbf{s}_{ \mathbf{x} \mathbf{y} } $$ corresponding to the constant.) Therefore, those sample averages need to be computed just once in order to obtain the regression coefficients and related statistics.

##### Solution

(1) According to (1.2.5'),

$$
\mathbf{b} = \mathbf{S}_{\mathbf{x} \mathbf{x}}^{-1}
\mathbf{s}_{\mathbf{x} \mathbf{y}}.
$$

(2)

$$
\begin{align}
  \mathrm{SSR} & = \mathbf{e}' \mathbf{e}
  \qquad
  \text{(definition (1.2.12))}
  \\
  & = 
  (\mathbf{y} - \mathbf{X} \mathbf{b})'
  (\mathbf{y} - \mathbf{X} \mathbf{b})
  \qquad
  \text{(definition (1.2.4))}
  \\
  & =
  \mathbf{y}'\mathbf{y} - \mathbf{y}' \mathbf{X}
  \mathbf{b} - \mathbf{b}' \mathbf{X}' \mathbf{y}
  + \mathbf{b}' \mathbf{X}' \mathbf{X} \mathbf{b}
  \\
  & =
  \mathbf{y}'\mathbf{y} - \mathbf{y}' \mathbf{X}
  \mathbf{b} - \mathbf{b}' \mathbf{X}' \mathbf{y}
  + \mathbf{b}' \mathbf{X}' \mathbf{y}
  \qquad
  \text{(definition (1.2.5))}
  \\
  & =
  \mathbf{y}'\mathbf{y} - (\mathbf{X}' \mathbf{y})'
  \mathbf{b}
  \\
  & =
  n \cdot \mathbf{y}' \mathbf{y} / n - n \cdot
  \mathbf{s}_{\mathbf{x} \mathbf{y}}'
  \mathbf{S}_{\mathbf{x} \mathbf{x}}^{-1}
  \mathbf{s}_{\mathbf{x} \mathbf{y}}
  \\
  & =
  n \cdot ( \mathbf{y}' \mathbf{y} / n -
  \mathbf{s}_{\mathbf{x} \mathbf{y}}'
  \mathbf{S}_{\mathbf{x} \mathbf{x}}^{-1}
  \mathbf{s}_{\mathbf{x} \mathbf{y}} ).  
\end{align}
$$

(3)

$$
s^2 = \frac{\mathrm{SSR}}{n - K} = 
\frac{n}{n - K} \cdot ( \mathbf{y}' \mathbf{y} / n -
\mathbf{s}_{\mathbf{x} \mathbf{y}}'
\mathbf{S}_{\mathbf{x} \mathbf{x}}^{-1}
\mathbf{s}_{\mathbf{x} \mathbf{y}} ).
$$

(4)

$$
\begin{align}
  R^2 & = 1 - \frac{ \mathrm{SSR} }
  { \sum_{i=1}^n (y_i - \bar{y})^2 }
  \qquad
  \text{(definition (1.2.18))}
  \\
  & =
  1 - \frac{ \mathrm{SSR} }
  { \sum_{i=1}^n (y_i^2 - 2\bar{y}y_i + \bar{y}^2) }
  \\
  & =
  1 - \frac{ \mathrm{SSR} }
  { \sum_{i=1}^n y_i^2 - 2 \bar{y} \sum_{i=1}^n y_i
  + \sum_{i=1}^n \bar{y}^2 }
  \\
  & =
  1 - \frac{ \mathrm{SSR} }
  { n \cdot \mathbf{y}' \mathbf{y} / n
  - 2n \cdot \bar{y}^2 + n \cdot \bar{y}^2}
  \\
  & =
  1 - \frac{ \mathrm{SSR} }
  { n \cdot \mathbf{y}' \mathbf{y} / n
  - n \cdot \bar{y}^2}.
\end{align}
$$

---

Copyright ©2017 by Qiang Gao