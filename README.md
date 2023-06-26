# Deep-Learning-Model-Market-Sentiment-Analysis
### Market Sentiment Analysis on Tokopedia Product with NLP Model

#### Project Overview
In this notebook, we will delve into text cleaning for product reviews written in Indonesian language and subsequently implement an NLP model with GRU and LSTM layers. The objective is to classify the reviews into one of three categories: Negative, Neutral, and Positive Sentiment.

#### Data
The data was obtained from Kaggle and uploaded as product_reviews.csv. The data is about product reviews in Indonesian from Tokopedia.

Data field description:
| Columns | Meaning |
| --- | --- |
| text | feedback given from the users who have bought the product|
| rating | star rating given for the product |
| category | category of the product on Tokopedia platform |
| product_name | name of the product on Tokopedia platform |
| product_id | unique ID for the product |
| sold | number of product sold |
| shop_id | unuqie ID for the seller on Tokopedia platform |
| product_url | the link to the product |

#### Notebook Stucture
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

#### Methodology
- [ ] Text pre-processing
  - using NLTK
  - Sastriwi dictionary
  - own made dictionary for   

#### Result and Evaluation
![Words Sentiment](https://github.com/andreetanjung/Deep-Learning-Model-Market-Sentiment-Analysis/assets/123824152/61a71800-9bdb-400c-b02c-0fa5761e524f)
Above is the most common words on each sentiment.

I am comparing the GRU and LSTM layer models to achieve better results. The LSTM layer model outperforms the GRU model because, despite not having superior categorical accuracy, it exhibits less overfitting. 

![Gru Tunning](https://github.com/andreetanjung/Deep-Learning-Model-Market-Sentiment-Analysis/assets/123824152/b1019146-d634-4027-8edd-b07834067d49)
<sub> Gru with Tunning Result <sub>

![LSTM Tunning](https://github.com/andreetanjung/Deep-Learning-Model-Market-Sentiment-Analysis/assets/123824152/19de465f-32e3-45d4-b065-a2b1b7e6fc68)
<sub> LSTM with Tunning Result <sub>

It is evident that both models are experiencing underfitting, resulting in a modest ROC AUC score of 57.5%. This suggests that the models face challenges in effectively differentiating between sentences of varying sentiments. Several factors contribute to this subpar performance, including the lack of adequate text preprocessing. Indonesian comments often contain abbreviations and diverse writing styles, making it crucial to address these linguistic nuances during preprocessing.

#### Future Work 
For future work, for Indonesian words especially, we can use manual computing rather than using model. So first we can identify the most common words for each sentiment, put them in lists. And create a function that manually count how many words are corresponding to each sentiment.

#### Deployment
Model deployment link https://huggingface.co/spaces/andreetanjung/Milestone2_Phase2
