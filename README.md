# Evaluating Machine Learning Models with Confusion and Weighted Error Matrices

Computing the cost of different models (false positives vs. false negatives) using their weighted [confusion matrix].

---

## Problem Overview

Confusion matrices are often used to evaluate the performance of machine learning models. Model predictions resulting in true positives (TP) and true negatives (TN) indicate how precise the model is. Meanwhile, false positives (FP) and false negatives (FN) reveal the number of mistakes committed by the model.

In most real scenarios, however, different types of errors have different costs. For instance, when a model is evaluating if a pacient has a disease and it makes a wrong prediction, it is better that the prediction ends up being a false positive than a false negative. It is more acceptable to have a healthy pacient getting treatment than to have a diseased patient not receiving any help.

## Analysis Introduction

In this project, we load up a dataset having weather information for Australia. The objective here is to predict if it is going to rain in the next day. We train two models to make predictions, [Naive Bayes] and [Random Forest]. The models have different performance with respect to FP and FN rate. 

We examine the performance of each model by attributing weights for both types of prediction mistakes (FPs and FNs), like in the image below. In the end, Naive Bayes outperforms the more complex Random Forest model. Naive Bayes' prediction has less false negatives, the conventional worst type of mistake in weather prediction: saying that it is not going to rain when it is.

![weighted_error_matrix](https://user-images.githubusercontent.com/33037020/181660344-ff1111c0-47d9-448e-b517-93dec227fa25.png)

[//]: #

[confusion matrix]: <https://www.sciencedirect.com/topics/engineering/confusion-matrix>
[Naive Bayes]: <https://www.kdnuggets.com/2020/06/naive-bayes-algorithm-everything.html>
[Random Forest]: <https://www.kdnuggets.com/2020/01/random-forest-powerful-ensemble-learning-algorithm.html>
