# Scikit-Learn (sklearn):

Scikit-learn is a library in Python that provides many unsupervised and supervised learning algorithms. It’s built upon some of the technology like NumPy, pandas, and Matplotlib!
<hr/>
The functionality that scikit-learn provides include:

* Regression, including Linear and Logistic Regression
* Classification, including K-Nearest Neighbors
* Clustering, including K-Means and K-Means++
* Model selection
* Preprocessing, including Min-Max Normalization
<hr/>

## Why Scikit-Learn?
* Has many in-built machine learning models.
* Methods to evaluate machine learning models.
* Very well-designed API.
<hr/>

## Scikit-Learn workflow:

1. Getting the data ready.
2. Choose the right estimator/algorithm for our problem.
3. Fit the model/algorithm and use it to make predictions on our data.
4. Evaluating a model.
5. Improve a model.
6. Save and load a trained model.
<hr/>

## How to Convert Categorical Data to Numerical Data?

This involves two steps:
* Integer Encoding
* One-Hot Encoding

`1. Integer Encoding`

As a first step, each unique category value is assigned an integer value.

For example, “red” is 1, “green” is 2, and “blue” is 3.

This is called a label encoding or an integer encoding and is easily reversible.

For some variables, this may be enough.

The integer values have a natural ordered relationship between each other and machine learning algorithms may be able to understand and harness this relationship.

For example, ordinal variables like the “place” example above would be a good example where a label encoding would be sufficient.

`2. One-Hot Encoding`

For categorical variables where no such ordinal relationship exists, the integer encoding is not enough.

In fact, using this encoding and allowing the model to assume a natural ordering between categories may result in poor performance or unexpected results (predictions halfway between categories).

In this case, a one-hot encoding can be applied to the integer representation. This is where the integer encoded variable is removed and a new binary variable is added for each unique integer value.

In the “color” variable example, there are 3 categories and therefore 3 binary variables are needed. A “1” value is placed in the binary variable for the color and “0” values for the other colors.

<hr/>


## References:
`Scikit Documentation:` https://scikit-learn.org/stable/user_guide.html

`Machine Learning map:` https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html

`Seaborn:` https://seaborn.pydata.org/introduction.html
