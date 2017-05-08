# Solutions to Econometrics

by Qiang Gao, updated at Apr 23, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 3 Finite-Sample Properties of OLS

...

#### Review Question 1.3.2 (Example of a linear estimator)

For the consumption function example in Example 1.1, propose a linear and unbiased estimator of $$ \beta_2 $$ that is different from the OLS estimator.

##### Solution

We propose an estimator $$ \widehat{\beta}_2 = ( CON_2 - CON_1 ) / ( YD_2 - YD_1 ) $$.

1. When $$ YD_1, \ldots, YD_n $$ is known, $$ \widehat{\beta}_2 $$ is a linear combination of $$ CON_1, \ldots, CON_n $$.

2. Because

$$
\begin{align}
  \mathrm{E} ( \widehat{\beta}_2 | YD_1, \ldots, YD_n )
  & =
  \mathrm{E} \left( \left.
  \frac{ ( \beta_1 + \beta_2 YD_2 + \varepsilon_2) - ( \beta_1 + \beta_2 YD_1 + \varepsilon_1 ) }
  { YD_2 - YD_1 }
  \right| YD_1, \ldots, YD_n
  \right)
  \\
  & =
  \mathrm{E} \left( \left.
  \frac{ \beta_2 (YD_2 - YD_1) + \varepsilon_2 - \varepsilon_1 }
  { YD_2 - YD_1 }
  \right| YD_1, \ldots, YD_n
  \right)
  \\
  & =
  \beta_2 + 0 - 0 = \beta_2,
\end{align}
$$

So $$ \widehat{\beta}_2 $$ proposed here is linear and unbiased.

---

Copyright ©2017 by Qiang Gao