# Polynomial Regression

[Home](https://github.com/JorgeToT/Machine-Learning-Python-R)

Example: [Polynomial Regression](polynomial_regression.ipynb)

$$y=\alpha_1x+\alpha_2x^2+\alpha_3x^3+...+\alpha_nx^n$$

```python
from sklearn.preprocessing import PolynomialFeatures
poly_reg = PolynomialFeatures(degree = 4)
X_poly = poly_reg.fit_transform(X)
lin_reg_2 = LinearRegression()
lin_reg_2.fit(X_poly, y)
```


