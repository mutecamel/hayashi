# Solutions to Econometrics

by Qiang Gao, updated at Mar 13, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 1 The Classical Linear Regression Model

...

#### Review Question 1.1.1 (Change in units in the semi-log form)

In the wage equation

$$
\log ( WAGE_i ) = \beta_1 + \beta_2 S_i + \beta_3 TENURE_i + \beta_4 EXPR_i + \varepsilon_i,
\tag{1.1.3}
$$

of Example 1.2, if $$ WAGE $$ is measured in cents rather than in dollars, what difference does it make to the equation?

##### Solution

Let $$ WAGE' $$ denote the $$ WAGE $$ variable measured in cents, that is,

$$
WAGE' = 100 WAGE,
$$

$$
\log ( WAGE' ) = \log (100) + \log ( WAGE ).
$$

Substituting into equation (1.1.3),

$$
\log ( WAGE_i') - \log (100) = \beta_1 + \beta_2 S_i +
\beta_3 TENURE_i + \beta_4 EXPR_i +
\varepsilon_i,
$$

$$
\log (\mathit{WAGE}_i') = \log (100) + \beta_1 + \beta_2 S_i +
\beta_3 \mathit{TENURE}_i + \beta_4 \mathit{EXPR}_i +
\varepsilon_i,
$$

$$
\log ( WAGE_i') = \beta_1' + \beta_2 S_i + \beta_3
 TENURE_i + \beta_4 EXPR_i + \varepsilon_i,
$$

where $$ \beta_1' $$ is defined as $$ \beta_1' = \log (100) + \beta_1 $$. So the _only_ difference is $$ \beta_1 $$ is increased by $$ \log (100)$$.

---

Copyright ©2017 by Qiang Gao