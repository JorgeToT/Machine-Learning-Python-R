# Machine Learning with Python and R

* Part 1: Data Preprocessing
  * [Preprocessing](/Part%201%20-%20Data%20Preprocessing/Python/)
    * [Example](/Part%201%20-%20Data%20Preprocessing/Python/data_preprocessing_tools.ipynb)

* Part 2: Regression models
  * [Simple Linear Regression Model](/Part%202%20-%20Regression/Section%204%20-%20Simple%20Linear%20Regression/Python/)
    * [Example](/Part%202%20-%20Regression/Section%204%20-%20Simple%20Linear%20Regression/Python/simple_linear_regression.ipynb)
    * Form: $y = \alpha x + \beta$
  * [Multiple Linear Regression Model](/Part%202%20-%20Regression/Section%205%20-%20Multiple%20Linear%20Regression/Python/)
    * [Example](/Part%202%20-%20Regression/Section%205%20-%20Multiple%20Linear%20Regression/Python/multiple_linear_regression.ipynb)
    * Form: $y = \alpha_1 x_1 + \alpha_2 x_2 + \alpha_3 x_3 + ... \alpha_n x_n + \beta$
  * [Polynomial Regression Model](/Part%202%20-%20Regression/Section%206%20-%20Polynomial%20Regression/Python/)
    * [Example](/Part%202%20-%20Regression/Section%206%20-%20Polynomial%20Regression/Python/polynomial_regression.ipynb)
    * Form: $y = \alpha_1 x + \alpha_2 x^2 + \alpha_3 x^3 + ... + \alpha_n x^n + \beta$
  * [Support Vector Regression (SVG) Model](/Part%202%20-%20Regression/Section%207%20-%20Support%20Vector%20Regression%20(SVR)/Python)
    * [Example](/Part%202%20-%20Regression/Section%207%20-%20Support%20Vector%20Regression%20(SVR)/Python/support_vector_regression.ipynb)
    * Like the Linear Regression Model, the SVR model is a linear model that is used to predict the value of a dependent variable as a function of the values of the independent variables. Have $\epsilon$ be the error margin.
  * [Decision Tree Regression Model](/Part%202%20-%20Regression/Section%208%20-%20Decision%20Tree%20Regression/Python/)
    * [Example](/Part%202%20-%20Regression/Section%208%20-%20Decision%20Tree%20Regression/Python/decision_tree_regression.ipynb)
  * [Random Forest Regression Model](/Part%202%20-%20Regression/Section%209%20-%20Random%20Forest%20Regression/Python/)
    * [Example](/Part%202%20-%20Regression/Section%209%20-%20Random%20Forest%20Regression/Python/random_forest_regression.ipynb)
    * A random forest is a set of decision trees that are used to predict the value of a dependent variable as a function of the values of the independent variables.

* Part 3: Classification models
  * [Logistic Regression Model](/Part%203%20-%20Classification/Section%2014%20-%20Logistic%20Regression/Python/)
    * [Example](/Part%203%20-%20Classification/Section%2014%20-%20Logistic%20Regression/Python/logistic_regression.ipynb)
    * This model provides a classification model with a lineal separator. The lineal separator is a line that separates the two classes of data.
  * [K-Nearest Neighbors (K-NN) Model](/Part%203%20-%20Classification/Section%2015%20-%20K-Nearest%20Neighbors%20(K-NN)/Python)
    * [Example](/Part%203%20-%20Classification/Section%2015%20-%20K-Nearest%20Neighbors%20(K-NN)/Python/k_nearest_neighbors.ipynb)
    * This model calculate the distance between the data and the nearest neighbor. The nearest neighbor is the data point that is closest to the data.
  * [Support Vetor Machine (SVM) Model](/Part%203%20-%20Classification/Section%2016%20-%20Support%20Vector%20Machine%20(SVM)/Python)
    * [Example](/Part%203%20-%20Classification/Section%2016%20-%20Support%20Vector%20Machine%20(SVM)/Python/support_vector_machine.ipynb)
    * SVM works by mapping data to a high-dimensional feature space so that data points can be categorized, even when the data are not otherwise linearly separable.
  * [Kernel SVM](/Part%203%20-%20Classification/Section%2017%20-%20Kernel%20SVM/Python)
    * [Example](/Part%203%20-%20Classification/Section%2017%20-%20Kernel%20SVM/Python/kernel_svm.ipynb)
    * Types of Kernel functions: 
      * Gaussian RBF Kernel. $K(x,l^i) = e^{-\frac{1}{2}(\frac{x-l^i}{\sigma})^2}$
      * Sigmoid Kernel. $K(x,y) = tanh(\gamma X^T + r)$ 
      * Polynomial Kernel. $K(x,y) = (\gamma X^T Y + r)^d$
  * [Naive Bayes Classifier](/Part%203%20-%20Classification/Section%2018%20-%20Naive%20Bayes/Python/)
    * [Example](/Part%203%20-%20Classification/Section%2018%20-%20Naive%20Bayes/Python/naive_bayes.ipynb)
  * [Decision Tree Classification](/Part%203%20-%20Classification/Section%2019%20-%20Decision%20Tree%20Classification/Python/)
    * [Example](/Part%203%20-%20Classification/Section%2019%20-%20Decision%20Tree%20Classification/Python/decision_tree_classification.ipynb)
  * [Random Forest Classification](/Part%203%20-%20Classification/Section%2020%20-%20Random%20Forest%20Classification/Python/)
    * [Example](/Part%203%20-%20Classification/Section%2020%20-%20Random%20Forest%20Classification/Python/random_forest_classification.ipynb)

* Part 4: Clustering
  * [K-Means Clustering](/Part%204%20-%20Clustering/Section%2024%20-%20K-Means%20Clustering/Python/)
    * [Example](/Part%204%20-%20Clustering/Section%2024%20-%20K-Means%20Clustering/Python/k_means_clustering.ipynb)
    * This model is used to cluster data points into groups. The groups are represented by a set of centroids.
    * Works better in large data sets.
  * [Hierarchical Clustering](/Part%204%20-%20Clustering/Section%2025%20-%20Hierarchical%20Clustering/Python/)
    * [Example](/Part%204%20-%20Clustering/Section%2025%20-%20Hierarchical%20Clustering/Python/hierarchical_clustering.ipynb)
    * This model join the closest clusters together to form a new cluster.

* Part 5: Association Rule Learning
  * The Association Rule Learning (ARL) model is used to discover association rules. It means that it finds the rules that are most likely to be true.
  * [Apriori](/Part%205%20-%20Association%20Rule%20Learning/Section%2028%20-%20Apriori/Python/)
    * [Example](/Part%205%20-%20Association%20Rule%20Learning/Section%2028%20-%20Apriori/Python/apriori.ipynb)