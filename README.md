# MBTI Prediction
Comparison between various ML models to determine personality type (MBTI) based on some text people have written using Scikit-Learn

In this project, dataset containing comments from different people with different personalities is available on kaggle. The goal of the project is to classify the comments based on the writers personalities. The personalities are determined based on The Myers–Briggs Type Indicator (MBTI). several models are used for the classification to see which one performs better.

# About MBIT itself!
The Myers–Briggs Type Indicator (MBTI) is one of the most famous questionaries that determines a persons personality. MBTI states that what appears to be random variance in behavior is really fairly regular and consistent, owing to fundamental variations in how people prefer to utilize their sense and judgment. MBTI made up of four different opposing categories, Introversion (I) – Extroversion (E), Intuition (N) – Sensing (S), Thinking (T) – Feeling (F), and Judging (J) – Perceiving (P). Therefore, 4 charachter are assigned to each person as the MBTI personality type. 

People behave due to their personality, and there are certain charachterstics that each personality is presented with [4]. Consequently, it is crusial for people to know their partner, friends, or family members personalities in order to respond properly to their actions. As it takes lots of time and effort to find out a person personality type, having a tool that can predict personality types based on available data such as comments, tweets, or text messages is essential. 

# Dataset
We use a dataset containing comments and the personality type of their writers. In the pre-processing step, we first clean the data by removing the usless stuff (the things unrelated to the comment text) such as links and emails. We also exclude the meaningless words such as 'a', 'the', etc with the help of NLTK library. Finally, we extract some features from the dataset such as number of words, number of nouns, number of question marks, number of links per comment, number of music per comment, number of verbs, number of image per comment, number of exclamation marks, and number of ellipsis. 

# Approach
We train different machine learning approaches with the extracted features. These methods include: K-Nearest Neighbours (KNN), Logistic Regression (LR), Neural Networks (NN), Naive Bayes,and SVM. In addition, we used 2 different approaches for the classification. First, we tried to predict the whole personality type by having 16 different classes. However, due to the inbalancy of data in the dataset, the models could not perform well. Then, we changed the approach by considering 4 different binary classes, e.g. Introverted and Extroverted. The second approach perfomed much better than the first one. 
