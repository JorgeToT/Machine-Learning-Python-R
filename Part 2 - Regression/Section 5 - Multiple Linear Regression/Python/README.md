# Multiple Lineal Regression

[Home](https://github.com/JorgeToT/Machine-Learning-Python-R)

Example: [Multiple Linear Regression](multiple_linear_regression.ipynb)

$$y=\alpha_1 x_1+\alpha_2 x_2+\alpha_3 x_3+...+\alpha_nx_n+\beta$$

As the Simple Linear Regression Model we need to minimize the sum of the squared errors, or with the R-squared or Adjusted R-squared to select the best model.

After the preprocessing (Import libraries, Missing Values, Transform categorical data, split to data and test sets and Scale the data) we can create the model with `LinearRegression` and fit it to the training data.

```python
from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
regressor.fit(X_train, y_train)
```

At last we use the model to predict the values using the test data of $X$ and compare the data between reuslts of the model and the test data for $y$

```python
y_pred = regressor.predict(X_test)
np.set_printoptions(precision=2)
print(np.concatenate((y_pred.reshape(len(y_pred),1), y_test.reshape(len(y_test),1)),1))
```

Now we can graph the results of the model to visualize the results.