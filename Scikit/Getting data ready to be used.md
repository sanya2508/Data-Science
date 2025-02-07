# Getting our data ready to be used with machine learning

## Three main things we have to do:

1. Split the data into features and labels (usually `X` & `y`)

2. Filling (also called imputing) or disregarding missing values.

3. Converting non-numerical values to numerical values (also called feature encoding).

<hr/>

## Extension: Feature Scaling

Once your data is all in numerical format, there's one more transformation you'll probably want to do to it.

It's called Feature Scaling.

In other words, making sure all of your numerical data is on the same scale.

For example, say you were trying to predict the sale price of cars and the number of kilometres on their odometers varies from 6,000 to 345,000 but the median previous repair cost varies from 100 to 1,700. A machine learning algorithm may have trouble finding patterns in these wide-ranging variables.

### To fix this, there are two main types of feature scaling.

* `Normalization (also called min-max scaling) `- 

This rescales all the numerical values to between 0 and 1, with the lowest value being close to 0 and the highest previous value being close to 1. Scikit-Learn provides functionality for this in the MinMaxScalar class. https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MinMaxScaler.html

* `Standardization` - 

This subtracts the mean value from all of the features (so the resulting features have 0 mean). It then scales the features to unit variance (by dividing the feature by the standard deviation). Scikit-Learn provides functionality for this in the StandardScalar class. https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html


#### A couple of things to note.

* Feature scaling usually isn't required for your target variable.

* Feature scaling is usually not required with tree-based models (e.g. Random Forest) since they can handle varying features.

#### Other references

* https://medium.com/@rahul77349/feature-scaling-why-it-is-required-8a93df1af310

* https://benalexkeen.com/feature-scaling-with-scikit-learn/

* https://www.analyticsvidhya.com/blog/2020/04/feature-scaling-machine-learning-normalization-standardization/

<hr/>

### Some takeaways:

* Split your data first (into train/test), always keep your training & test data separate

* Fill/transform the training set and test sets separately (this goes for filling data with pandas as well)

* Don't use data from the future (test set) to fill data from the past (training set)

<hr/>

#### SimpleImputer is a scikit-learn class which is helpful in handling the missing data in the predictive model dataset. It replaces the NaN values with a specified placeholder.

It is implemented by the use of the SimpleImputer() method which takes the following arguments :

* missing_values : The missing_values placeholder which has to be imputed. By default is NaN

* stategy : The data which will replace the NaN values from the dataset. The strategy argument can take the values – ‘mean'(default), ‘median’, ‘most_frequent’ and ‘constant’.

* fill_value : The constant value to be given to the NaN data using the constant strategy.
