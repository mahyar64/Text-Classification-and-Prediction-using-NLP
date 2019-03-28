#  Text  Classification and Prediction using NLP

For runnign Machine Learning (ML) models on the data for classification, prediction or detection we use these steps:

1.   Collecting, loading, and cleaning data
2.   Build your model
3.   Train the data
4.   Evaluation & Prediction

###Question 
Propose a model of ML to read the data from dataset, understand and make a prediction fomr the text which contains the chatbot/call conversation of a Bank costomers. There are two files, 'Training_Dataset.xlsx' for training and 'Validation_dataset.csv' for testing and eveluations. 

##Implementation platform and reading 
In the first step, I read and load data locally. For the implementation due to being independent from installing python libraries such as Tensorflow and Keras,
I used colaboratory from Google which is a jupyter notebook file (https://colab.research.google.com). 
Data can be read directly from colab page. 

##Cleaning and exploring the data-set 
After reading the dataset, I had a look to see how many categories are in the data set and how many attribute is there for each category.
The graphs show the differences.
Recent process is done for both training and evaluation data. There are 28 different categories in training data-set.
While there are 29 categories in the test set. It means there is a category in the evaluation data that is not represented 
in training set. I removed it due to make more precise validation and prediction accuracy.
The class which is not seen during the training can not be in the test.

##Text cleaning and pre-processing
Furthermore, I did some text cleaning to improvove the quality of training with removing not useful and not important words and characters
such as stop words,  punctuation, bad characters, change text to lower case. A sample of training data-set is presented before and after cleaning text processing.

##Build Machine Learning models
Subsequently, I defined a pipeline model with using 4 different ML algorithms.

1.  Naive Bayes Classifier
2.  Logistic Regression
3.  Stochastic Gradient Descent (SGD)
4.  Neural Network (Deep Learning)

The accuracy of prediction for any of above models are 0.58, 0.71, 0.73 and 0.97 respectively. 
