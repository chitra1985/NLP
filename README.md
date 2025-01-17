# NLP
## Amazon Review - Sentimental Analysis
Welcome to the sentimental Analysis! This project aims to perform sentimental analysis on customer review of Amazon  using NLP (Natural Language Processing). This README.md will guide you the key concepts of this project.
### Introduction to Sentimental Analysis
Sentiment analysis, also known as opinion mining, is a natural language processing (NLP) technique used to determine the emotional tone behind a piece of text. The primary goal of sentiment analysis is to identify whether a given text expresses positive, negative, or neutral sentiment. It involves analyzing various textual features to classify the sentiment conveyed by the text.
### Usage and importance
Sentiment analysis has numerous applications across different domains:

* __Business Insight__ : Companies can use sentiment analysis to gauge public opinions about their products, services, and brand, helping them make informed decisions.
* __Social Media Monitoring__ : Sentiment analysis is widely used to monitor social media platforms to understand public sentiment about various topics in real-time.
* __Customer Feedback__ : It aids in analyzing customer feedback and reviews to improve products and services based on user experiences.
* __Market Research__ : Sentiment analysis can provide insights into market trends and consumer preferences by analyzing discussions and reviews.
* __Political Analysis__ : It can be used to understand public sentiment about political candidates, policies, and events
### Data Collection
- The dataset used for this project is sourced from __Kaggle__, prominent online platform for data scientists and machine learning practitioners.
- The specific dataset used for this project titled "Amazon Customer Review Dataset"
### Text Preprocessing
Text preprocessing is crucial for effective sentimental analysis.
* __Lower casing__ : In the first step of NLP project, we converted the comments in Title column to lower case. This standardize the data into uniform format, eliminating inconsistency in case sensitivity during text processing.
* __Punctuation Removal__ : In this step, we remove the punctuations from the 'Title' column. This process aims to enhance the efficiency of our text processing task by making our text data cleaner and understand to analysis.
* __Numbers Removal__ : In this step, we remove the numbers from the 'Title' column. By removing numbers, our text processing task make our text data cleaner and more meaningful data analysis.
* __StopWord Removal__ : In this step, by removing frequently repeated or often meaningless words ('is', 'the','in'), from text, we can focus on meaningful words which will improve our NLP oerformance.
* __Rarewords Remval__ : In this step, we combine all the comments or review in th 'Title' column, then split the resulting text into words, then count the frequency of the each word. In this process we identified the words that appear only once.subsequently we remvoe the rare words from the column will improve the NLP model focus on more significant words.
* __Tokenization__ : In this part, we transformed all the comment/review in the 'Title' column into TextBlop object and then tokenize them into words. TextBlops easily split the comment into tokens.This process enable us to examine each words in each comment and conduct more detailed NLP analysis based on the words.
* __Lemmanitation__ : In this step, we lemmatize each review in the 'Title' column to its root or base word. Lemmatization reduces different forms of words. This provide more cosistent and meaning data processing in NLP analysis.

These preprocessing steps effectively cleaned the text data, removed irrelevant information, and prepared it for feature extraction and subsequent model training. By carefully cleaning and preparing the text, we aimed to improve the accuracy and robustness of the sentiment analysis model.
### Text Visualization
* __WordCloud__ : In this section, we create and visualize a word cloud using the review from the 'Title' column. The purpose is to display the frequently occurring words in the dataset in a visual forma. This allows for a quick observation of the key trends and prominent features in the text data.
### Future Engineering
It is the process of extracting features from raw data. In this, we are converting each word into vector because meachine learning models only understand Numbers. In NLP we also call it as Text Representation.
* __CountVectorization__ : With this technique each review was then represented as a vector where each element corresponds to the frequency of a specific word in that review. Count Vectorization is simple to implement and computationally efficient.
* __TF-IDF__ : **Term Frequency (TF)**  measures how frequently a word appears within a specific document. **Inverse Document Frequency (IDF)** measures how rare a word is across the entire corpus. Words that appear in many documents are given lower weights. TF-IDF gives more weight to words that are important within a specific document but rare across the entire corpus.

By carefully selecting and applying appropriate text representation techniques, we can effectively transform the raw text data into meaningful numerical features that can be used to train accurate sentiment analysis models.
  

