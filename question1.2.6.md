# Solution to Review Question

by Qiang Gao, updated at Mar 21, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 2 The Algebra of Least Squares

...

#### Review Question 1.2.6 (Change in units and $$ R^2 $$)

Does a change in the unit of measurement for the dependent variable change $$ R^2 $$? A change in the unit of measurement for the regressors? **Hint:** Check whether the change affects the denominator and the numerator in the definition for $$ R^2 $$.

##### Solution

By definition,

$$
R^2 = \frac{ \sum_{i=1}^n (\hat{y}_i - \bar{y})^2 }
{ \sum_{i=1}^n (y_i - \bar{y})^2 }.
$$

(1) If we change the unit of measurement of the dependent variable $$ y $$, then $$ y_i $$, $$ \hat{y}_i $$, and $$ \bar{y} $$ simultaneously scales by a factor $$ \alpha $$. Both the denominator and the numerator are scaled by $$ \alpha^2 $$, leaving $$ R^2 $$ unchanged.

(2) If we change the unit of measurement of the regressors, then $$ y_i $$, $$ \hat{y}_i $$, and $$ \bar{y} $$ donnot change at all. $$ R^2 $$ remains unchanged.

---

Copyright ©2017 by Qiang Gao