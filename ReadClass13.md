# Read Topics: 13

## Linear Regression

### ***Concept:***

Linear regression is a  technique used to model the relationship between a dependent variable (also called the response variable) and one or more independent variables.

In the context of machine learning, linear regression is often used as a supervised learning algorithm. Given a dataset with known input-output pairs, the algorithm learns to predict the output value based on the input value. Once the algorithm is trained on the data, it can be used to make predictions on new, unseen data.

### ***Importing using Scikit Learn library:*** 

1- The first step is to import the necessary libraries, including NumPy, Pandas, and Scikit Learn. You can do this using the following code:

```
import numpy as np
import pandas as pd
from sklearn.linear_model import LinearRegression
```
2- The next step is to load the dataset you want to use to train the linear regression model. 

```
dataset = pd.read_csv('your_dataset.csv')
```
3- Next, you need to split the dataset into the dependent variable and the independent variable.

4-  Create a Linear Regression object.

```
regressor = LinearRegression()
```
5- Train the model on the training data.

6- Make predictions on the test data, and evaluate the model.

### ***Train & tests splits purpose:***

Splitting a dataset into training and test sets is a common practice in machine learning to evaluate the performance of a model. The purpose of doing this is to check how well the model is able to generalize to new, unseen data.

By evaluating the model on a separate test set, we can get a better idea of how well the model will perform on new, unseen data. If the model performs well on the test set, we can be more confident that it will perform well on new data.

