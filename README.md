# Sentiment-Analysis-on-Amazon-Fine-Food-Reviews 

## Objective:
In this project, I thoroughly explain the full pipeline of Natural Language Processing which includes - 
1. Text Pre-processing
    - Removing HTML Tags
    - Decontraction
    - Removing Special Characters & Punctuation
    - Removing Alphanumeric Words
    - Converting into Lower Case
    - Removing Stop Words
    - Stemming Words
2. Text Featurization
    - Bag of Words (BoW)
      - Simlpe Bag of Words (Uni/Bi-gram)
      - Term Frequency-Inverse Document Frequency (TF-IDF) Weighted Bag of Words (Uni/Bi-gram)
    - Word2Vec (Pre-Trained Model and Own Model)
      - Simple Average Word2Vec
      - Term Frequency-Inverse Document Frequency (TF-IDF) Weighted Average Word2Vec (Uni/Bi-gram)
3. Data Visualization using T-Distributed Stochastic Neighborhood Embedding (T-SNE)
    - On Bag of Words (BoW) representation (Uni-gram & Bi-gram)
    - On Term Frequency-Inverse Document Frequency (TF-IDF) Weighted Bag of Words (Uni-gram & Bi-gram)
    - On Simple Average Word2Vec
    - On Term Frequency-Inverse Document Frequency (TF-IDF) Weighted Average Word2Vec (Uni-gram & Bi-gram)
4. Prediction Using K-Nearest Neighbor Algorithm
    - On Bag of Words (BoW) representation (Uni-gram & Bi-gram)
    - On Term Frequency-Inverse Document Frequency (TF-IDF) Weighted Bag of Words (Uni-gram & Bi-gram)
    - On Simple Average Word2Vec
    - On Term Frequency-Inverse Document Frequency (TF-IDF) Weighted Average Word2Vec (Uni-gram & Bi-gram)
    
## Dataset Used:
Data Source: https://www.kaggle.com/snap/amazon-fine-food-reviews <br>

EDA: https://nycdatascience.com/blog/student-works/amazon-fine-foods-visualization/


The Amazon Fine Food Reviews dataset consists of reviews of fine foods from Amazon.<br>

Number of reviews: 568,454<br>
Number of users: 256,059<br>
Number of products: 74,258<br>
Timespan: Oct 1999 - Oct 2012<br>
Number of Attributes/Columns in data: 10 

Attribute Information:

1. Id
2. ProductId - unique identifier for the product
3. UserId - unqiue identifier for the user
4. ProfileName
5. HelpfulnessNumerator - number of users who found the review helpful
6. HelpfulnessDenominator - number of users who indicated whether they found the review helpful or not
7. Score - rating between 1 and 5
8. Time - timestamp for the review
9. Summary - brief summary of the review
10. Text - text of the review

## Conclusion:
The F1 Scores for various representations when KNN was used - 
1. BoW 
    - Uni-gram ==> 0.728 (k=31)
    - Uni+Bi-gram ==> 0.765 (k=21)
2. TF-IDF Weighted BoW
    - Uni-gram ==> 0.781 (k=71)
    - Uni+Bi-gram ==> 0.781 (k=69)
3. Word2Vec
    - Uni-gram Average Word2Vec ==> 0.786 (k=53)
    - TF-IDF Weighted Average Word2Vec
      - Uni-gram ==> 0.761 (k=71)
      - Uni+Bi-gram ==> 0.761 (k=25)

