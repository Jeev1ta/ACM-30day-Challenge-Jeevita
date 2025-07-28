# Tweet Sentiment Analysis Breakdown – Phase 5 Summary
## Steps Performed:
- Loaded the dataset and selected relevant columns (sentiment and tweet text).
- Cleaned the tweets by removing URLs, mentions, hashtags (kept words), special characters, and converting text to lowercase.
- Mapped sentiment labels from numeric (0, 2, 4) to more intuitive categories: Negative (0), Neutral (1), Positive (2).
- Converted tweet text into numerical format using TF-IDF Vectorization, capturing the importance of words with a vocabulary size limit.
- Split the data into training and test sets and trained a classification model (e.g., Logistic Regression / SVM / Naive Bayes / XGBoost).
- Evaluated the model using Accuracy, Confusion Matrix, and Classification Report (Precision, Recall, F1-score).

## Key Learnings:
- Learned how to process and clean large-scale tweet data by removing noise and standardizing text for analysis.
- Understood how TF-IDF transforms text into meaningful numeric vectors by emphasizing important words across documents.
- Saw how machine learning models can be trained to classify sentiment based on features extracted from text.
- Gained experience in evaluating model performance using metrics like F1-score and visual tools like Confusion Matrices to interpret errors.

I worked on Tweet Sentiment Analysis using the Sentiment140 dataset, applying Natural Language Processing (NLP) techniques and machine learning. I learned how to clean and preprocess large-scale text data, convert it into meaningful numerical features using TF-IDF, and train models like Logistic Regression and Naive Bayes for classification. I also practiced evaluating model performance using accuracy, precision, recall, and F1-score. This deepened my understanding of how text data can be analyzed and modeled to extract sentiment and patterns in real-world social media content.


## Write-up
I used Logistic Regression because it’s fast, easy to use, and works well for text data like tweets.
TF-IDF helped turn the tweets into numbers by giving more importance to unique words in each tweet. This made it easier for the model to learn which words are linked to positive, negative, or neutral feelings.
A big challenge was cleaning the tweets, like removing links, usernames, and emojis. I fixed this using some Python code with regular expressions. Also, since the full dataset is huge, I worked with a smaller sample to save time while still getting good results.
