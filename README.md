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
Due to the lack of resources for labeling in Arabic and the absence of sentiment labels in the original dataset,  the text was translated into English using the googletrans library, before being annotated with TextBlob for sentiments.

## 2. Preprocessing:
There are various procedures involved in preprocessing tweets for sentiment analysis. Any special characters, digits, URLs, and Twitter identities were first removed. Second, to maintain uniformity, all text is changed to lowercase. The tweets are then tokenized, which involves separating them into separate words or tokens. The tokens are then lemmatized to return them to their original forms.

## 3. Feature Extraction:
Feature extraction was used to vectorize data by converting preprocessed text into numerical data using TF-IDF.

## 4. Classification:
For sentiment analysis, many classification models were used, including Nave Base, logistic regression, SVM, neural networks, and Random Forest. Then, to analyze the model, we used accuracy to determine how well the classifier performs in predicting the sentiments of the tweets.

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

