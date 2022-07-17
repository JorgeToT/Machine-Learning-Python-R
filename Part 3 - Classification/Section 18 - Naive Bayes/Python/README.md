# Naive Bayes
By using the Naive Bayes algorithm, we can classify a new data point based on the existing data.

It based on the assumption that the probability of a data point belonging to a class is proportional to the probability of the data point belonging to each of the features in the class.


Bayes theorem:
$$P(A|X) = \frac{P(X|A)P(A)}{P(X)}$$

* $P(A|X)$ Posterior probability of A given X
* $P(X|A)$ Likelihood of X given A
  * Probability of a similar values belongs at a A class
* $P(A)$ Prior probability of A
* $P(X)$ Marginal likelihood of X
  * Probability of the similar values belongs at a X class

Given a data point, we can calculate the probability of the data point belonging to each class. And the maximum probability will be the class of the data point. This is called the naive bayes algorithm.

To create a naive bayes classifier we need to have X and y data, then separate the data into training and testing data and scale the data.

After this we trainthe model:
    
```python
from sklearn.naive_bayes import GaussianNB
classifier = GaussianNB()
classifier.fit(X_train, y_train)
```

To predict we can use the following code:
    
```python
print(classifier.predict(sc.transform([[30,87000]])))
```
In this case the output will be 1.

To finish we can comparate the test data with the predicted data.
