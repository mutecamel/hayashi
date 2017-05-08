# Solutions to Econometrics

by Qiang Gao, updated at Mar 20, 2017

---

## Chapter 1 Finite-Sample Properties of OLS

### Section 2 The Algebra of Least Squares

...

#### Review Question 1.2.1

Prove that $$ \mathbf{X}' \mathbf{X} $$ is positive definite if $$ \mathbf{X} $$ is of full column rank. 

##### Solution

By the definition of positive definite matrix, we need to show that $$ \mathbf{c}' \mathbf{X}' \mathbf{X} \mathbf{c} > 0 $$ for $$ \mathbf{c} \neq \mathbf{0} $$. Define $$ \mathbf{z} \equiv \mathbf{X} \mathbf{c} $$. Then $$ \mathbf{c}' \mathbf{X}' \mathbf{X} \mathbf{c} = \mathbf{z}' \mathbf{z} = \sum_{k=1}^{K} z_i^2 $$. If $$ \mathbf{X} $$ is of full column rank, then the column vectors of $$ \mathbf{X} $$ are linearly independent. This means $$ \mathbf{X} \mathbf{c} = \mathbf{0} $$ if and only if $$ \mathbf{c} = \mathbf{0} $$. Then $$ \mathbf{z} \neq \mathbf{0} $$ for any $$ \mathbf{c} \neq \mathbf{0} $$.

---

Copyright ©2017 by Qiang Gao