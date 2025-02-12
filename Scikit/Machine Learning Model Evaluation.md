# Machine Learning Model Evaluation
## Evaluating the results of a machine learning model is as important as building one.

But just like how different problems have different machine learning models, different machine learning models have different evaluation metrics.

Below are some of the most important evaluation metrics you'll want to look into for classification and regression models.

## Classification Model Evaluation Metrics/Techniques

`Accuracy` - The accuracy of the model in decimal form. Perfect accuracy is equal to 1.0.

`Precision` - Indicates the proportion of positive identifications (model predicted class 1) which were actually correct. A model which produces no false positives has a precision of 1.0. (https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_score.html#sklearn.metrics.precision_score)

`Recall` - Indicates the proportion of actual positives which were correctly classified. A model which produces no false negatives has a recall of 1.0. (https://scikit-learn.org/stable/modules/generated/sklearn.metrics.recall_score.html#sklearn.metrics.recall_score)

`F1 score` - A combination of precision and recall. A perfect model achieves an F1 score of 1.0. (https://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html#sklearn.metrics.f1_score)

`Confusion matrix` - Compares the predicted values with the true values in a tabular way, if 100% correct, all values in the matrix will be top left to bottom right (diagonal line). (https://www.dataschool.io/simple-guide-to-confusion-matrix-terminology/)

`Cross-validation` - Splits your dataset into multiple parts and train and tests your model on each part then evaluates performance as an average. (https://scikit-learn.org/stable/modules/cross_validation.html)

`Classification report` - Sklearn has a built-in function called `classification_report()` which returns some of the main classification metrics such as precision, recall and f1-score. (https://scikit-learn.org/stable/modules/generated/sklearn.metrics.classification_report.html)

`ROC Curve` - Also known as receiver operating characteristic is a plot of true positive rate versus false-positive rate. (https://en.wikipedia.org/wiki/Receiver_operating_characteristic)

`Area Under Curve (AUC) Score` - The area underneath the ROC curve. A perfect model achieves an AUC score of 1.0. (https://scikit-learn.org/stable/modules/generated/sklearn.metrics.roc_auc_score.html)

## Which classification metric should you use?

* Accuracy is a good measure to start with if all classes are balanced (e.g. same amount of samples which are labelled with 0 or 1).

* Precision and recall become more important when classes are imbalanced.

* If false-positive predictions are worse than false-negatives, aim for higher precision.

* If false-negative predictions are worse than false-positives, aim for higher recall.

* F1-score is a combination of precision and recall.

* A confusion matrix is always a good way to visualize how a classification model is going.

## Regression Model Evaluation Metrics/Techniques

* R^2 (pronounced r-squared) or the coefficient of determination - Compares your model's predictions to the mean of the targets. Values can range from negative infinity (a very poor model) to 1. For example, if all your model does is predict the mean of the targets, its R^2 value would be 0. And if your model perfectly predicts a range of numbers it's R^2 value would be 1. (https://scikit-learn.org/stable/modules/generated/sklearn.metrics.r2_score.html)

* Mean absolute error (MAE) - The average of the absolute differences between predictions and actual values. It gives you an idea of how wrong your predictions were. (https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_absolute_error.html)

* Mean squared error (MSE) - The average squared differences between predictions and actual values. Squaring the errors removes negative errors. It also amplifies outliers (samples which have larger errors). (https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_squared_error.html)

## Which regression metric should you use?

* R2 is similar to accuracy. It gives you a quick indication of how well your model might be doing. Generally, the closer your R2 value is to 1.0, the better the model. But it doesn't really tell exactly how wrong your model is in terms of how far off each prediction is.

* MAE gives a better indication of how far off each of your model's predictions are on average.

* As for MAE or MSE, because of the way MSE is calculated, squaring the differences between predicted values and actual values, it amplifies larger differences. Let's say we're predicting the value of houses (which we are).

* Pay more attention to MAE: When being $10,000 off is twice as bad as being $5,000 off.

* Pay more attention to MSE: When being $10,000 off is more than twice as bad as being $5,000 off.


## For more resources on evaluating a machine learning model, be sure to check out the following resources:

* Scikit-Learn documentation for metrics and scoring (quantifying the quality of predictions) (https://scikit-learn.org/stable/modules/model_evaluation.html)

* Beyond Accuracy: Precision and Recall by Will Koehrsen (https://towardsdatascience.com/beyond-accuracy-precision-and-recall-3da06bea9f6c?gi=ce361c8f0215)

* Stack Overflow answer describing MSE (mean squared error) and RSME (root mean squared error) (https://stackoverflow.com/questions/17197492/is-there-a-library-function-for-root-mean-square-error-rmse-in-python/37861832#37861832)
