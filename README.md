# KSA-Telecom-Customer-Arabic-Sentiment-Analysis
The project intends to analyze Saudi Telecom customers' sentiments based on tweets to the company's customer care account. The dataset used for this analysis is the 'customer care tweets KSA' dataset from Kaggle in the Arabic language, which has severe processing challenges and a lack of labeling tools and resources. Tweet preprocessing, sentiment labeling, feature extraction, and sentiment classification are the four primary stages of the project.

# Install Necessary Libraries
! pip install emoji

! pip install googletrans==3.1.0a0

# Dataset:
The project utilizes the "customer care tweets KSA" dataset from Kaggle, containing 10,000 tweets from a telecom business customer service account. This dataset has no labels associated with it.

Link: [customer care tweets KSA on Kaggle]([https://www.kaggle.com/datasets/mansourhussain/customer-care-tweets-ksa])

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
Preprocessing of 14485 tweets out of 14640 was successful. There were 5415 positive, 3632 negative, and 5438 neutral tweets total, which were divided into three groups.

<img src="./images/Pie_Chart.png">

<img src="./images/stack_chart.png">

Numerous classification models were used to train the sentiment analysis model, including Nave Base, logistic regression, SVM, neural networks, and Random Forest. Random Forest, whose accuracy was 98%, had the highest level of precision.

<img src="./images/Classifiers_Performance.png">

With a low number of false positives, the confusion matrix for Random Forest showed significant accuracy in sentiment categorization.

## Technologies Used:
List the languages, libraries, and tools used in the project.

## Contact:
Your contact info or a link to your GitHub profile for those who might have questions or collaboration ideas.

