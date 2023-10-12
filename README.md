# KSA-Telecom-Customer-Arabic-Sentiment-Analysis
The project intends to analyze Saudi Telecom customers' sentiments based on tweets to the company's customer care account. The dataset used for this analysis is the 'customer care tweets KSA' dataset from Kaggle in the Arabic language, which has severe processing challenges and a lack of labeling tools and resources. Tweet preprocessing, sentiment labeling, feature extraction, and sentiment classification are the four primary stages of the project.

# Install Necessary Libraries
! pip install emoji

! pip install googletrans==3.1.0a0

# Dataset:
The project utilizes the "customer care tweets KSA" dataset from Kaggle, containing 10,000 tweets from a telecom business customer service account. This dataset has no labels associated with it.

Link: [customer care tweets KSA on Kaggle](https://www.kaggle.com/datasets/mansourhussain/customer-care-tweets-ksa)

# Methodology
The sentiment analysis project was organized into the following essential stages:

## 1. Labeling:
The text was translated into English using the googletrans library before being annotated using TextBlob for sentiments due to the lack of Arabic labeling resources and the absence of sentiment labels in the original dataset.

## 2. Preprocessing:
Tweet sentiment analysis requires some preprocessing steps. The text is cleaned by removing any non-alphabetic characters, links, and usernames. Next, the text is split into tokens, which are individual words or units. Finally, the tokens are lemmatized to get their base forms.

## 3. Feature Extraction:
We applied feature extraction to transform the cleaned text into numeric data with TF-IDF. This technique assigns weights to words based on their frequency and importance in the documents.

## 4. Classification:
Random Forest classifications were employed for sentiment analysis. After that, to evaluate the model, we calculated the accuracy and confusion matrices to assess how well the classifier performed at predicting the sentiments of the tweets.

## Results:
- The preprocessing step resulted in 9748 tweets out of 10,000 being ready for further analysis.

- The analysis showed that customer sentiment was neutral for 5520 tweets, positive for 2627 tweets, and negative for 1601 tweets.

<img src="./images/Pie_Chart.png">

The sentiment analysis model was trained using a Random Forest classifier, which achieved an accuracy of 73.2%. This is a reasonable performance considering the complexity and variability of Arabic language data.

<img src="./images/Classifiers_Performance.png">


