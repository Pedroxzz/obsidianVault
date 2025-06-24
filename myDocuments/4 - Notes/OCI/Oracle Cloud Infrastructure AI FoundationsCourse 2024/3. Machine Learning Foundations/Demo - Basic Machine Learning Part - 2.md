---
tags:
  - oci
Index: "[[3. Machine Learning Foundations]]"
---
# Transcript 
First of all, I'm going to make a duplicate of this existing file and will rename it as MLDemo. So click on this duplicate. And then I can rename this as 2. Since we are not going to use this notebook anymore, I can close the tab and shut down. Let's open MLDemo2.

In this new notebook, let's start by adding few more libraries, which we need. Before that, click on the Kernel. Restart and clear all the outputs. Let's import the libraries, which we will need for this section of the demo.

We have imported NumPy library and aliased it as a NP. NumPy is used for numerical computations and provides arrays and mathematical functions. Again, we have imported a train test split function from scikit-learn model selection module. So this function is used to split the data set into training and testing sets.

We have imported the standard scalar class from the scikit-learn's pre-processing module. So this class is used to standardize the features by scaling them to have a mean of 0 and standard deviation of 1. We import the accuracy score function from scikit-learn's metrics module. So this function is used to calculate the accuracy of model predictions. So let's understand what these libraries are exactly doing.

Let's take the case of this standardization. Standardization is the process of transforming data so that it has mean of 0 and a standard deviation of 1. It's important in machine learning because it ensures that all features or variables are on the same scale. Preventing some features from dominating the learning process due to their largest magnitude.

For example, let's say you are building a machine learning model to predict house prices, and you have two features-- square footage and number of bedrooms. The square footage values-- let's say it ranges from 1,000 to 5,000 square feet. While the number of bedrooms ranges from 1 to 6.

So, in case if you don't standardize these features, the model might give more weight to a square footage because it has larger values. And this could result in an inaccurate model as the number of bedrooms might also be a significant predictor. So the standardization scales both those features to have comparable means and standard deviation and hence, allowing the model to treat them equally.

Coming on to this train test split, this is a helpful to divide the data into a training set and a test set. And now you can train your model on the training set and evaluate its accuracy on the testing set. This accuracy score here-- this is a metric used to measure the accuracy of a classification model. It calculates the ratio of correctly predicted instances to the total number of instances in the data set.

This is important part of validation, which is the process of evaluating a machine learning model's performance on a separate data set, which we call as validation set to ensure it generalizes well and does not overfit the training data.

To explain this, for example, let's say you are building a spam email classifier, which will basically classify your email as spam or not spam. So after training your model, you use a validation set. Usually, the email is not seen during the training process to calculate the accuracy using this accuracy score. If accuracy is 95%, it means your model correctly classifies 95% of email as a spam or not spam. So the validation overall ensures your model performs well on the new unseen data and helps you avoid building a model that only works on the training data.

And that latter case is called as overfitting. Following the previous demo, we will now load the data set and display some rows and split the data set into feature x and labels y. These libraries have been successfully imported. So now we will run the next two consecutive cells.

As the next step, we will further split the data into training and test sets, meaning we will have x divided into x train, x test, and y divided into y train and y test. So let's paste the code for the same. You also notice that there is a parameter called randomstate. So this parameter is often used to control the randomness.

So what I mean by that, that when you use this train test split from sklearn and set randomstate, for example, equals to 42. The data splitting will be random, but reproducible. So if you run the same code with same randomstate value again, you will get the same split of the data. And this is useful for the reproducibility and for comparing results between different experiments.

So let's now run this cell block. We will now standardize our features. So we will add a cell here. This is the code for standardization of the features. In the first line, we are creating an instance of the standard scalar class, which will be used to standardize the features.

Next, we'll follow the same code as previously we did. We will create an ML model. So we'll create an instance of logistic regression model. But now in the next step, instead of you just training the model on x and y, we will use the newly scaled data using this fit method. So let's replace this code.

So now, on running this code, we have trained the logistic regression model using the standardized training features x trained skill and the corresponding training labels y train. Model learns the relationship between the features and the labels during this step. Once trained before predicting the values, let's evaluate our model on the testing set.

So basically, let's see how our model is performing on the unseen data once it has learned the patterns from the training data. Here, we have used the trained model to make predictions on the standardized testing features, which is x test scale and this line produces a set of predicted labels for this testing data.

We will calculate the accuracy of the model's predictions by comparing this predicted labels with the true labels from the testing set. The accuracy score function provides the accuracy as a metric. Generally speaking, higher the accuracy score is that means your model is better.

So we have got the accuracy of 1, that means this is 100% accurate. We will create a sample new data for the prediction. So this is the code for creating a sample new data for prediction using NumPy.

I will assume that these data points represent the attributes of Iris flowers, which we want to classify. It can be entirely new data points or examples for which we want to predict the species. This length-- the sepal length is this first column. The sepal width is this next column. This petal length and petal width is again respectively the other two columns.

And then what we are trying to do here guess the species. And this is a new data for prediction. The model haven't seen this data yet. We will again start with standardizing this new data samples. This is the code. Let me run the cell block. We have standardized the new data in the same way that we did for the training and testing data. Let's make predictions.

Squad will help you to make predictions, and we use the trained models to make predictions on the standardized new data points. The model will now predict the species of Iris flower based on their attributes. I will display the predicted classes on the basis of this sample new data.

Let's run this cell, and you can see that these are the respective predicted classes as per this sample new data for prediction. The first attributes combination-- this has been classified as Iris setosa. And similarly, for the other two, it is classified as Iris virginica and Iris setosa again.

This extended demo-- we covered all the additional steps, such as offdata preprocessing, some model evaluation, and making predictions on the new data. Again, this reflects a more comprehensive machine learning workflow. As you continue to explore machine learning, you will find that these steps are crucial for building effective models. This concludes our demo. I hope it will be helpful for your future endeavors in machine learning. So Thank you for joining.