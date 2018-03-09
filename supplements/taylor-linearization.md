## Taylor's Linearization

by Qiang Gao, updated at Mar 9, 2018

---

Any nonlinear differentiable function, i.e., a curve of points $$(y, x)$$, depicted as $$y = f(x)$$, can be _locally_ approximated as a line, called **linearization**, around any point $$(\bar{y}, \bar{x})$$ on the curve.

#### One Independent Variable Case

A function of a single variable $$y = f(x)$$ can be approximately linearized around a point $$(\bar{y}, \bar{x})$$, where $$\bar{y} = f(\bar{x})$$, as

$$
y - \bar y \approx \frac{d f(\bar{x})}{d x} (x - \bar x_1).
$$

#### Two Independent Variable Case

A function of two variables $$y = f(x_1, x_2)$$ can be approximately linearized around a point $$(\bar{y}, \bar{x}_1, \bar{x}_2)$$, where $$\bar{y} = f(\bar{x}_1, \bar{x}_2)$$, as

$$
y - \bar{y} \approx \frac{\partial f(\bar{x}_1, \bar{x}_2)}{\partial x_1} (x_1 - \bar{x}_1) + \frac{\partial f(\bar{x}_1, \bar{x}_2)}{\partial x_2} (x_2 - \bar{x}_2).
$$

#### Many Independent Variable Case

A function of $$K$$ independent variables $$y = f( \mathbf{x})$$, where $$\mathbf{x} = (x_1, x_2, \ldots, x_K)$$, can be approximately linearized around point $$(\bar{y}, \bar{ \mathbf{x} })$$, where $$\bar{y} = f( \bar{ \mathbf{x} } )$$, as

$$
y - \bar{y} \approx \nabla f(\bar{ \mathbf{x} }) \cdot ( \mathbf{x} - \bar{ \mathbf{x} } ).
$$

---

Copyright ©2018 by Qiang Gao