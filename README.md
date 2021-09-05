# Deep-Learning-and-Nlp-for-disaster-detection
# Problem Statement
Let’s go through the problem statement once as it is very crucial to understand the objective before working on the data.The problem statement is as follows:

The dataset train.csv contains 7613 rows and 5 columns.Our objective is to train a deep learning model by using Natural Language Processing  which detects disasters.

# Procedure implemented in acheiving our objective:
Load required libraries.

Load train.csv into dataframe df.

use 're' module in python for defining two functions remove_url and remove_punc for replacing urls with ' ' and removing  punctuations respectively.

Apply these two functions to text column of the df dataframe.

Import nltk library for removing  stopwords and then split the text into words by converting all the words into lower.

By using counter from collections library we can count total  number of unique words.

Now divide data into train and validation sets.

Now using tensorflow's tokenizer divide the train sentences and validation sentences into tokens.

Now give train and validation tokens into pad sequences function by giving padding='post attribute to it for setting padding.

Create a LSTM model,compile and fit the training data by giving validation_data as validation data.

We acheived accuracy of 98.46 which is pretty good.
So we need not to do any hyperparameter tuning and fix to this model for doing predictions.











