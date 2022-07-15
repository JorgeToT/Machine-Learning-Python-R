# Simple Linear Regression Model

[Home](https://github.com/JorgeToT/Machine-Learning-Python-R)

Example:
[Simple Linear Regression](simple_linear_regression.ipynb)

$$y=\alpha x+\beta$$

The model tries to minimize the sum of the squared errors. It means we have to minimize $\sum_0^n |y(x) - y|$, and the model whose have the minimum sum of the squared errors is the best model.

Other way to select the best model is maximize R-squared.

$$R^2 = {\sigma^2_{xy} \over \sigma_x^2 \sigma_y^2}$$

But for more precision we have to considerate Adjusted R-squared, wich based on the number of observations and the number of variables.

$$Adjusted R^2 = {1 - {(1-R^2)(N-1) \over N - p - 1}}$$

For this model we need to considerate the following:

* ${2 \over 3}$ of the data is used to train the model.
* ${1 \over 3}$ of the data is used to test the model.

As we see previously to separate the data we need to use the `train_test_split` function.

```python
from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 1/3, random_state = 0)
```

After split the data, we create the model with `LinearRegression` and fit it to the training data.

```python
from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
regressor.fit(X_train, y_train)
```

Now we use the model to predict the values using the test data of $X$ and compare the data between reuslts of the model and the test data for $y$

```python
y_pred = regressor.predict(X_test)
```

After this we can graph the results of the model.