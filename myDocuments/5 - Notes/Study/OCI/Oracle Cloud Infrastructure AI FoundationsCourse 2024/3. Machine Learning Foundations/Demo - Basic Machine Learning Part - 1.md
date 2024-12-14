---
tags:
  - oci
Index: "[[3. Machine Learning Foundations]]"
---
# Transcript 
Before we implement a machine learning use case, let's revisit a typical machine learning process, which involves loading of the data, preprocessing the data, training a model, evaluating the model, and making predictions. ## Machine learning process. I'll convert it to Markdown. The code which we will write will demonstrate a simple machine learning workflow using logistic regression, which is a classifier.

In machine learning, a classifier is a type of algorithm or model that is used for the task of classification. Classification is a supervised learning problem where the goal is to assign a category or label to a given input based on its features. Again, the primary purpose of a classifier is to learn patterns and relationships in the training data so that it can make predictions or decisions about the category or label of new unseen data points.

Our code will load the data, will prepare it for training, will train a model, and will make prediction and print the results. The example which we will be using is a very foundational example of how machine learning models are built and used for classification tasks. So let's begin.

We will start with importing some Python and ML libraries, which we will need to run codes. Let's first import some libraries. Now, I will add a comment # Import necessary Libraries. OK. So the first line here, this line imports the pandas library, and aliases it as a pd. pandas is used for data manipulation and provides data structures like dataframes and series for handling data efficiently.

The second line this imports the logistic regression class from scikit learn or sklearn library. This scikit learn is a popular machine learning library that provides tool for data pre-processing, model training, and evaluation. If you run this cell, you might not be able to successfully import these libraries if these are not the part of your kernel. And to install these libraries to your notebook kernel, go back to your previous page. And in the New item open a terminal. This page will pop up here.

And then on this page, you can copy paste this particular command. I copied it from the installation section from this packages scikit-learn. So conda install -c anaconda scikit-learn. If all goes well, you will see a page like this. And this will prepare or verify and execute your transaction and will add that library to your kernel.

Once I run this code, we have successfully imported all the necessary libraries. Next, we will load our data set. We will load the data set and display the first few rows. We use pandas to read a CSV file named iris.csv and store it in a dataframe called iris_data. This line loads the data set into memory and making it available for analysis.

This data set often called the iris data set contain information about different species of iris flowers. And this is how the iris.csv file looks. So you can see it has different columns the attributes. If we run this code, now you can see the same iris_data dataframe shows the first five rows on running this particular line. A head method is used to inspect the data set and get a quick overview of its content. This is a very helpful step to understand the structure of your data.

In the next step, we will split the data into features X and label Y. The features denoted as X contains the attributes of the iris flowers while the labels denoted as Y represents the species of the iris. So we also got rid of the ID, this column, which is not a useful attribute for the flower. It's just a numbering for our rows.

In this line, we create a new dataframe, as I said, X by dropping the ID and Species column from iris_data. And the next line we are going to create a series Y that contains the Species columns from the iris_data dataframe. This represents the target variable of labels. Let's run this cell. You can also check how those looks. So X looks like X is a dataframe and Y is a series. So which we'll have the corresponding target levels for each of these rows.

In the next step, we will create a machine learning model. So as I discussed about logistic regression, this is a classifier. In this demo, we will initialize it as model=LogisticRegression() method using this LogisticRegression class we imported earlier. This line initializes the model with default settings.

Next will come the training part. So in this step, we will train our model. This fit method is called to train the logistic regression model on features X and their corresponding labels Y This steps involves learning the relationship between the features and the target variable. So let's run this code. Once our model is trained, next comes the predictions.

So let's make prediction on a few data points. You can see these data points here, this will act as an attribute for, let's say, unseen data. OK, let's run this cell. Now, let's print the prediction to the console. This line here will display the predicted species of iris flower based on these given input feature values.

The predictions on the basis of these inputs came out to be Iris-setosa. So in this demo, we loaded a data set, we split it into features and labels, created a machine learning model, trained that model, and use it to make predictions and print those predictions on our console. So I hope this demo will be helpful, and now we will move on to the next demo.