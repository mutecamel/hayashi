# Solutions to Econometrics

by Qiang Gao, updated at Mar 21, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 2 The Algebra of Least Squares

...

#### Review Question 1.2.7 (Relation between $$ R_{uc}^2 $$ and $$ R^2 $$)

Show that

$$
1 - R^2 = \left( 1 + \frac{ n \cdot \bar{y}^2 }{ \sum_{i=1}^n (y_i - \bar{y})^2 } \right)
(1 - R_{uc}^2).
$$

**Hint:** Use the identity $$ \sum_i (y_i - \bar{y})^2 = \sum_i y_i^2 - n \cdot \bar{y}^2 $$.

##### Solution

By definition of $$ R^2 $$, the left side equals

$$
\frac{ \sum_{i=1}^n e_i^2 }{ \sum_{i=1}^n (y_i - \bar{y})^2 }.
$$

By definition of $$ R_{uc}^2 $$, the right side equals

$$
\begin{align}
  & \left( 1 + \frac{ n \cdot \bar{y}^2 }
  { \sum_{i=1}^n (y_i - \bar{y})^2 } \right)
  \frac{ \sum_{i=1}^n e_i^2 }{ \sum_{i=1}^n y_i^2 }
  \\
  = &
  \left( \frac{ \sum_i y_i^2 - n \cdot \bar{y}^2 
  + n \cdot \bar{y}^2 }
  { \sum_{i=1}^n (y_i - \bar{y})^2 } \right)
  \frac{ \sum_{i=1}^n e_i^2 }{ \sum_{i=1}^n y_i^2 }
  \qquad
  \text{(hint)}
  \\
  = &
  \left( \frac{ \sum_i y_i^2  }
  { \sum_{i=1}^n (y_i - \bar{y})^2 } \right)
  \frac{ \sum_{i=1}^n e_i^2 }{ \sum_{i=1}^n y_i^2 }
  \\
  = &
  \frac{ \sum_{i=1}^n e_i^2 }{ \sum_{i=1}^n 
  (y_i - \bar{y})^2 }.
\end{align}
$$

Left side and right side are equal.

---

Copyright ©2017 by Qiang Gao