# Solution to Review Question

by Qiang Gao, updated at Mar 13, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 1 The Classical Linear Regression Model

...

#### Review Question 1.1.5 (Multicollinearity for the simple regression model)

Show that Assumption 1.3 for the simple regression model is that the nonconstant regressor ($$ x_{i2} $$) is really nonconstant (i.e. $$ x_{i2} \neq x_{j2} $$ for some pairs of $$ (i, j) $$, $$ i \neq j $$, with probability one).

##### Solution

The simple regression model is

$$
\mathbf{y} = \beta_1 \cdot \mathbf{1} + \beta_2 \mathbf{x}_2 + \boldsymbol{\varepsilon}.
$$

Assumption 1.3 requires that $$ \{ \mathbf{1}, \mathbf{x}_2 \} $$ are linearly independent with probability one. This means $$ \mathbf{x}_2 $$ is not proportional to $$ \mathbf{1} $$ with probability one, i.e., $$ x_{i2} \neq x_{j2} $$ for some pairs of $$ (i, j) $$, $$ i \neq j $$, with probability one.

---

Copyright ©2017 by Qiang Gao