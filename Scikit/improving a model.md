 ## Improving a model

First predictions = baseline predictions. First model = baseline model.

### From a data perspective:

* Could we collect more data? (generally, the more data, the better)
* Could we improve our data?

### From a model perspective:

* Is there a better model we could use?
* Could we improve the current model?
* Hyperparameters vs. Parameters

<hr/>

Parameters = model find these patterns in data

Hyperparameters = settings on a model you can adjust to (potentially) improve its ability to find patterns
<hr/>

### Three ways to adjust hyperparameters:

* By hand
* Randomly with RandomSearchCV
* Exhaustively with GridSearchCV
