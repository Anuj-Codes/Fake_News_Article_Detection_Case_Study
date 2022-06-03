![Fake_News_Image](https://user-images.githubusercontent.com/92272579/171402715-33614ade-d967-471d-b030-5c453233cc56.png)

# Fake News Article Detection Case-Study
# Introduction

In an era where fake WhatsApp forwards and Tweets are capable of influencing naive minds.
What is Fake news?
Fake news's simple meaning is to incorporate information that leads people to the wrong path. Nowadays fake news spreads like water and people share this information without verifying it. This is often done to further or impose certain ideas and is often achieved with political agendas.
For media outlets, the ability to attract viewers to their websites is necessary to generate online advertising revenue. So it is necessary to detect fake news.
Based on their content, produced fake news is difficult to detect because the language used in fake news is very close to the language used in actual news, as fake news is created with the purpose to be trusted. 
Fake news identification from online social media is extremely challenging due to various factors. First, the collection of fake news data is difficult, and it is also difficult to manually label fake news.

# Business problem
This case study is about fake news detection and developing a machine learning program to identify when an article might be fake news.
This is one of the kaggle problem named as Fake News Build a system to identify unreliable news articles.

Kaggle url :-https://www.kaggle.com/competitions/fake-news/overview

# ML formulation of the business problem
Given a text Article, we have to identify whether it's a fake article or not.
It is Binary classification 1 for Fake or unreliable articles and 0 for not fake or reliable articles

# Deployed Fake News Detector Application

  ![image](https://user-images.githubusercontent.com/92272579/171403459-f495f5dd-5f30-4cab-98cd-63c63d22e78e.png)

My detailed approach can be viewed in this medium article.
# Results
| Sl No. | Model | Kaggle Private score | Kaggle Public score |
| - | --------------------- | ----------- |----------- |
| 1. | Gaussian NB | 0.87747 |0.88205
| 2. | Logistic Regression | 0.96483 |0.96794 
| 3. | Xgboost Classifier | 0.96895 |0.97179
| 4. | Decision Tree | 0.94917 |0.95448
| 5. | Lightgbm Classifier | 0.97472 |0.97435
| 6. | Voting Classififer(Soft) | 0.97307|0.97564

Contents of the Code Files are given below :-

| Code File | Description  | 
| ----  | --------- |
| Fake-News-Detection-EDA-Case-Study.ipynb    | Exploratory Data Analysis and Feature Engineering|
| Fake-News-First-Cut-Model-Building.ipynb    | Created first cut solution of problem using only text features|
| Fake-News-Modeling-Experimentation.ipynb    | Added 18 manually engineered features along with text features|
| Fake_News_Hyperparameter_tunning.ipynb   | Hyperparameter tunning of models|
| Fake-News-Final-Pipeline-Notebook.ipynb  | Function 1 - takes input X, returns prediction Y,Function 2 - takes input (X,Y) returns evaluation metric (Accuracy)|
| Final_testing_Deployed_Fake_news_Application_Demo.ipynb   | Demo of Fake news Application created using streamlit|
| voting.pkl   | Best Model saved after hypereparameter tunning|

