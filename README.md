Twitter Sentiment Analysis using NLTK, Python

Developed a simple Twitter Sentiment Analysis supervised learning model using python and NLP libraries.
Started by importing the required libraries for the project.
Read the data with pandas.

Perform Exploratory Data Analysis

Data preprocessing and Feature Engineering
The following techniques of preprocessing the raw data were tried. 
1. Removal of punctuations.
2. Removal of commonly used words (stopwords).
3. Normalization of words.
We need to do Lexicon Normalization approach. NLTK’s built-in WordNetLemmatizer does this requirement.

Vectorization and Model Selection
The well-known techniques for vectorization of words in Natural Language Processing are: CountVectorization and Tf-IDF transformation. 

Chose the naive bayes classifier for binary classification since it is the most common algorithm used in NLP.Next, used machine learning pipeline technique which is a built-in function of scikit-learn to pre-define a workflow of algorithm. This saves much time and computational power.

Model Validation
Used the conventional train_test_split technique to split the training data set.
Accuracy is measured using the built-in function of scikit-learn, confusion matrix and classification report.

The following accuracy is obtained : 
              precision    recall  f1-score   support

           0       1.00      0.93      0.97      6323
           1       0.14      1.00      0.25        70

    accuracy                           0.93      6393
   macro avg       0.57      0.97      0.61      6393
weighted avg       0.99      0.93      0.96      6393



[[5907  416]
 [   0   70]]
0.9349288284060692

