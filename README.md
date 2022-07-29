# Evaluating Machine Learning Models with Confusion and Weighted Error Matrices

Confusion matrices are often used to evaluate the performance of machine learning models. Model predictions resulting in true positives and true negatives indicate how precise the model is. Meanwhile, false positives and false negatives reveal the number of mistakes committed by the model.

In most real scenarios, however, different types of errors have different costs. Usually, when a model is evaluating if a pacient has a disease, if the model makes a false prediction, it is better that the prediction ends up being a false positive than a false negative. It is better to have a healthy pacient getting treatment than to have a diseased patient not receiving any help.

In this project, we load up a dataset having weather information for Australia. The objective here is to predict if it is going to rain in the next day. We train two models to make predictions, Naive Bayes and Random Forest. The models have different performance with respect to false positive (FP) and false negative (FN) rate. 

We examine the performance of each model by attributing weights for both types of prediction mistakes (FPs and FNs), like in the image below. In the end, Naive Bayes outperforms the more complex Random Forest because its prediction has less false negatives, the worst type of mistake in weather prediction.


![weighted_error_matrix](https://user-images.githubusercontent.com/33037020/181660344-ff1111c0-47d9-448e-b517-93dec227fa25.png)
