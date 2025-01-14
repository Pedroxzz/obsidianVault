---
tags:
  - oci
Index: "[[3. Machine Learning Foundations]]"
---
# Transcript 
Hello, and welcome to this lesson on supervised learning. In this lesson, we will discuss how classification works. In supervised machine learning model, the output can be either categorical or continuous. When the output is continuous, we use regression to predict a numeric output. And when the output is categorical, we use classification to predict a category or a label. We have seen regression earlier while building a house price predictor.

On the other hand, classification is a supervised learning problem where the goal is to assign a category or label to the outcome. If the classifier predicts whether an email is a spam or not, then it is an example of a binary classification. If we set up a model for sentiment prediction where a classifier can identify the positive, negative, and neutral sentiments in a given text, it is a multi-class classifier. Classification is a supervised machine learning technique used to categorize or assign data points into predefined classes or categories based on their features or attributes.

Classifier is trained on a labeled data set. For example, a classifier can be trained to detect a spam mail. The outcome in this case would be binary-- that is, if a mail is spam or not. Let us see one simple machine learning algorithm that is used for classification. It is called as logistic regression. Logistic regression predicts if something is true or false. Let us discuss a simple model of pass or fail among a set of students given the hours of study.

The input feature here is the hours of study, which is the independent variable, and the output is binary. That is pass or fail in this case. Depending on the hours of study, the student belongs to either pass class where he/she has passed the test or a failed class if he or she has failed the test. Unlike linear regression, which uses a straight line to fit the data, logistic regression uses an S-shaped curve called the sigmoid function to fit the data. The sigmoid function takes any real valued number and squashes it into a range between 0 and 1.

This property is essential for interpreting the output as a probability. In this case, we input hours of study to the sigmoid function, and we get corresponding probability of passing the test. Based on this probability, we can decide if it is a pass or fail decision. Output from the sigmoid function is to be compared with a threshold value of, say, 0.5. If output is more than 0.5, it would be classified as a pass. And if less than 0.5, it will be classified as a fail.

For example, a student who studies for six hours and having 80% probability to pass in the test is classified as "pass." A student who studies for four hours and have a 20% probability to pass the test is classified as "fail." In the upcoming demo, we use Iris data set. This is a standard machine learning data set having 150 instances of three types of Iris flowers, Iris setosa, Iris versicolor, and Iris virginica.

The flowers are characterized according to four attributes-- sepal length, sepal width, petal length, and petal width. Because there are three classes to be categorized on the basis of the input features, this is a case of multi-class classification. Logistic regression will be used to classify flowers in the upcoming demo. We have four features and a output label with three values representing the three classes. Thanks for watching.