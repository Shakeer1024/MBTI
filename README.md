# MBTI
This project is used to investigate if any patterns can be detected in a person’s specific personality type in connection to their text postings on a social forum, and to explore the validity of the test in analyzing and predicting or categorizing behavior using natural language processing techniques.

# Data Exploration:
1. There are 8675 rows and 2 columns in the dataframe.
2. Two Columns(types and posts) with no null values.
3. Type column contains 16 unique codes representing the 16 different personality types.
4. Each post is separated by 3 pipelines(|||) and on an average each type consists of nearly 50 posts.


# Data Cleaning:
1. Entry combing (Removing pipelines).
2. Removing Hyperlinks.
3. Removing Contractions.
4. Removing all the references of MBTI types used in posts.
5. Removing Punctuations and Digits.
6. Word Tokenizing.
7. Lemmatization.
8. Stop Words Removal.

# Data Analysis:
1. Frequency Distribution.
2. Top words before and after data cleaning.
3. Mean word count.
4. Investigating mean word count by axes.
5. Top 10 words in all Individual MBTI Types (Extrovert, Introvert, Intuition, Sensing, Thinking, Feeling, Judging, Perceiving).

# Model Selection
The following algorithms have been used for predicting the MBTI personality.
1. Random Forest Classifier
2. Logistic Regression
3. SGD (Stochastic Gradient Descent) Classifier and 
4. Artificial Neural Networks

Out of all the above models the SGD Classifierhas the highest accuracy score of 67%. And the next Logistic Regression with the predicting accuracy of 63% , Random Forest Classifier with least accuracy 55%.

# Conclusion
1. The model classifiers perform good when there is a representation of types in their data compared to when there is not. This is achieved by classifying the classes across all the 4 axes which helps in  reducing the noise in the data by allowing SGDClassifier to focus on only two hypothetically polar aspects of the data at a time
2. Within all the models the SGDClassifier has the highest accuracy of 67% followed by Logistic Regression with 64%.
3. Hopefully this analysis can serve as a strong reminder of the power of context. Text is something that is readily available in multitudes of observations, and is so often discarded as being too complex to be useful. From what we can see in this applied analysis, context can add a powerful element to what might otherwise be a useless bag of words, and when considered carefully enough can actually.

# Future Work
1. On top of predicting a person’s MBTI type, I hope to expand the project further by introducing video titles, image keywords which we can extract from the hyper links also Performing Sentiment analysis. 
2. Creating an application for predicting the personality type using Flask/Django Framework.

