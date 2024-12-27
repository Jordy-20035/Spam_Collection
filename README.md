SMS Spam Detection

Overview

This project implements a machine learning solution for detecting spam messages in SMS using Python. The model is trained on a dataset of SMS messages labeled as either "ham" (not spam) or "spam". The goal is to classify incoming messages accordingly, helping to filter out unwanted spam messages effectively.

Dataset

The dataset used in this project is a collection of SMS messages that can be found in the SMSSpamCollection file. Each message is labeled as "ham" or "spam".
Requirements
To run this project, the following Python libraries should be installed:

•	pandas

•	numpy

•	nltk

•	scikit-learn

•	matplotlib

Steps Implemented

1.	Data Loading: The dataset is loaded using pandas, with appropriate column names assigned.


2.	Data Exploration:
o	The structure of the dataset is examined, along with the distribution of 'ham' and 'spam' messages.

3.	Data Preprocessing:
o	The labels are encoded into binary format (ham: 0, spam: 1).
o	Text preprocessing is performed on the SMS messages, including:

  	Lowercasing the text.
  	Removing punctuation and special characters.
  	Removing stopwords using the NLTK library.
  
4.	Train-Test Split: The processed data is split into training and testing sets to evaluate the model performance.

5.	Text Vectorization: The text data is transformed into numerical format using the TF-IDF (Term Frequency-Inverse Document Frequency) vectorizer.
   
6.	Model Training: A Support Vector Classifier (SVC) is trained on the training set.
    
7.	Model Evaluation:

o	Predictions are made on the test set.

o	The model's performance is evaluated using metrics such as precision, recall, F1-score, and overall accuracy.

o	A confusion matrix is generated to visualize the performance of the model.

Results

•	The final model achieved an accuracy of 98%, indicating a high level of correct predictions.

•	The classification report provides insights into precision, recall, and F1-score for both classes (ham and spam).
