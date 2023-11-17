# Disaster Tweets Classification

## Overview
This project focuses on building a machine learning model to predict whether a tweet is about a real disaster or not. In today's digital age, Twitter has become a crucial communication channel during emergencies. The widespread use of smartphones allows individuals to report real-time observations of emergencies, making it a valuable source of information for disaster relief organizations and news agencies.

However, the challenge lies in distinguishing between tweets that genuinely announce a disaster and those that use disaster-related terms metaphorically or in different contexts. For instance:

![Example Tweet](https://imgur.com/a/ji0e6CM)

While the word "DISASTER" is used to express frustration and inconvenience related to heavy traffic, it doesn't imply an actual disaster like a natural calamity. In this context, the tweet is about a common, non-emergency situation. 
This ambiguity underscores the need for a reliable machine learning model capable of discerning the true nature of tweets during emergencies.

## Data
The dataset for this project is obtained from Kaggle and can be accessed directly on Kaggle's [NLP Getting Started Competition Data Page](https://www.kaggle.com/competitions/nlp-getting-started/data?select=train.csv).

### Sample Tweets. It includes a collection of tweets that have been manually classified into two categories:

- **Real Disasters (Target = 1):** Tweets associated with actual disasters or emergencies.
- **Non-Disasters (Target = 0):** Tweets that are not related to real disasters.


## Code
The Jupyter Notebook contains the entire code for data loading, preprocessing, model training, and evaluation. The key steps include:

1. Data Cleaning and Exploration: Checking for missing values and exploring the dataset.
2. Text Preprocessing: Cleaning the text data by removing URLs, HTML tags, and non-alphabetic characters. Tokenization and removal of stop words are also performed.
3. TF-IDF Vectorization: Transforming the cleaned text data into numerical features using TF-IDF vectorization.
4. Model Building: Creating an ensemble model using three classifiers - Multinomial Naive Bayes, Logistic Regression, and Support Vector Machine.
5. Model Evaluation: Assessing the model performance on a validation set, including accuracy, confusion matrix, and classification report.

## Results
The ensemble model achieved a validation accuracy of approximately 81.44%.Detailed metrics, including precision, recall, and F1 score, can be found in the classification report.

## Testing
The trained model is applied to the test dataset (`test.csv`), and the predictions are stored in `submission.csv`.



