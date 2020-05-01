# Six step Guide for Machine Learning Models

## 1. PROBLEM DEFINITION:

Define the problem. Is it regression or classification problem, supervised learning or unsupervised learning, etc?
Machine Learning isn’t the solution to every problem. The initial step is to match the problem you’re trying to solve a machine learning problem.
The four main types of Machine Learning are:
1. Supervised Learning: The main types of Supervised Learning are Classification (if something is one thing or the other) and Regression(predict the number).
2. Unsupervised Learning: These have data but no labels. These types of problems are also called Clustering.
3. Transfer Learning: Transfer learning leverages what one machine learning model has learned in another machine learning model. This is valuable because training a machine learning model from scratch can be very expensive.
4. Reinforcement Learning (not so common): It involves having a computer program perform some actions within a defined space and rewarding it for doing it well or punishing it for doing poorly.

## 2. DATA:
Define the kind of data that we have, and how does it align with the problem definition.
Data are generally present in either of two forms: Structured data or Unstructured data. Within each of two lies static data(Existing data which is unlikely to change) or streaming data(Data which is constantly updated).

## 3. EVALUATION:
Define success. Decide the percentage accuracy that would be good enough for the respective model.

## 4. FEATURES:
Decide what we already know about the data, and the part of the data we are going to use for our machine learning model. Can it be used to make predictions? The three main types of features are categorical, continuous (or numerical), and derived.

## 5. MODELLING:
Decide the model we should choose. Can it be improved further?
Modelling can be broken down into three parts:
1. Choosing and training a model.
2. Tuning a model (It involves changing hyperparameters or model-specific architecture factors).
3. Model Comparison (avoid overfitting and underfitting).

## 6. EXPERIMENTATION:
Does our machine learning model perform as we expected?
Poor performance on training data means the model hasn’t learned properly. Try a different model, improve the existing one, collect more data, collect better data.
Poor performance on test data means our model doesn’t generalize well. Our model may be overfitting the training data.
Poor performance once deployed (in the real world) means there’s a difference in what we trained and tested our model on and what is actually happening. Revisit step 1 & 2. Ensure that the data matches up with the problem we’re trying to solve.



## Other Important References

`Correlation matrix`: https://www.displayr.com/what-is-a-correlation-matrix/

`Statistics Course`: https://www.youtube.com/watch?v=zouPoc49xbk&list=PL8dPuuaLjXtNM_Y-bUAhblSAdWRnmBUcr

`Mathematics Course`: https://www.khanacademy.org/math

`CONDA documentation`: https://docs.conda.io/en/latest/

`Getting started with conda`: https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html

`Getting ready(MINICONDA)`: https://www.mrdbourke.com/get-your-computer-ready-for-machine-learning-using-anaconda-miniconda-and-conda/



