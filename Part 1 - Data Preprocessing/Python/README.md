# <center>Data preprocessing</center>

Example:
[Data preprocessing](/Part%201%20-%20Data%20Preprocessing/Python/data_preprocessing_tools.ipynb)

First steps:
We need to import libaries, import dataset.

```python
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd

dataset = pd.read_csv('')
X = dataset.iloc[:, :-1].values
y = dataset.iloc[:, -1].values
```

After this we can start preprocessing the data.
We have to check if exists any missing values in the dataset, for this we can use the following code:

```python
from sklearn.impute import SimpleImputer
imputer = SimpleImputer(missing_values=np.nan, strategy='mean')
imputer.fit(X[:, 1:3])
X[:, 1:3] = imputer.transform(X[:, 1:3])
```

Also we have to check if the data is categorical or not, for this we can use the following code:

```python
# Independent variables
from sklearn.compose import ColumnTransformer
from sklearn.preprocessing import OneHotEncoder
ct = ColumnTransformer(transformers=[('encoder', OneHotEncoder(), [0])], remainder='passthrough')
X = np.array(ct.fit_transform(X))

# Dependent variables
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
y = le.fit_transform(y)
```

At last we need to split the data into train and test sets as we can see in the code below.
    
```python 
from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size = 0.2, random_state = 0)
```

Another thing we have to do is to scale the data, for this we can use the following code:

$$ z = {x - \mu \over \sigma} $$

```python
from sklearn.preprocessing import StandardScaler
sc = StandardScaler()
X_train[:, 3:] = sc.fit_transform(X_train[:, 3:])
X_test[:, 3:] = sc.transform(X_test[:, 3:])
```

After all we can start training the model.