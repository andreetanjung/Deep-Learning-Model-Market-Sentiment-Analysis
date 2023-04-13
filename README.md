# Deep-Learning-Model-Market-Sentiment-Analysis
### Market Sentiment Analysis on Tokopedia Product with NLP Model
In this notebook, we will delve into text cleaning for product reviews written in Indonesian language and subsequently implement an NLP model with GRU and LSTM layers. The objective is to classify the reviews into one of three categories: Negative, Neutral, and Positive Sentiment.
Data field description:
  - text: feedback given from the users who have bought the product
  - rating: star rating given for the product
  - category: category of the product on Tokopedia platform
  - product_name: name of the product on Tokopedia platform
  - product_id: unique ID for the product
  - sold: number of product sold
  - shop_id: unuqie ID for the seller on Tokopedia platform
  - product_url: the link to the product

Here is the outline for the notebook:
  - Data Loading and Overview
  - General Data Cleaning
  - Exploratory Data Analysis
  - Text Pre-Processing
  - Handling Imbalance Data
  - Text Vectorization and Embedding
  - Modeling
  - Model Conclusion
  - Evaluation
