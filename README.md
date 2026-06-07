# Construction-of-an-additive-model-based-on-Kolmogorov-s-theorem

**Topic:** Recovering a Regression Relationship Using an Additive Model

This work considers the problem of recovering an unknown relationship

$$
y = f(x_1,\ldots,x_p) + \varepsilon,
\qquad x_j \in [0,1].
$$

Kolmogorov's representation theorem for continuous functions motivates the use of models in which a multivariate function is represented through sums and superpositions of univariate functions. In this laboratory work, we consider a computationally tractable special case — the **additive model**:

$$
\hat f(x) = \beta_0 + \sum_{j=1}^{p} g_j(x_j).
$$

The main objective of this study is to investigate how well such a model can recover nonlinear relationships from data, compare its performance with linear and fully nonlinear models, and analyze the effect of the number of basis functions on the approximation quality.

# 1. Experimental Setup

The notebook performs the following steps:

1. Generation of synthetic additive data.
2. Construction of the block feature matrix for the additive model.
3. Parameter estimation using ordinary least squares and ridge regression.
4. Centering of the components $\hat g_j$ to ensure unique interpretation.
5. Comparison with linear regression.
6. Comparison with a full polynomial model including interaction terms.
7. Investigation of the effect of the number of basis functions.
8. A separate experiment on non-additive data containing interactions between features.

