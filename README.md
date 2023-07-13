# ML-sentiment-analysis
Machine Learning (ML) project: Sentiment Classification of Tweets. 3 ML classifiers, Support Vector Machines (SVM), Logistic Regression (LR), and Naïve Bayes (NB) were tested on diferent combinations of features extracted from tweets for a final performance of 76.62% accuracy.

## Methodology Diagram
<img width="384" alt="Screen Shot 2023-07-13 at 23 43 52" src="https://github.com/patwdj/ML-sentiment-analysis/assets/80323885/0e06b2d6-0c11-4e20-bf25-050d231724c0">

## Data Required
Data provided as part of assigment has not been uploaded to this repository:
- Labelled training set of Tweets, a labelled development set, and an unlabeled test set. Each tweet is labelled with one of three possible sentiments (i.e., class labels), where pos, neg, and neu denote positive, negative, and neutral sentiments. Provided representations of Tweets:
  - full: The raw tweets represented as a single string, e.g.,
  ```
  tweet ID,“im feeling so happy today, so very happy”
  ```
  - count: stands for “Bag of Words”. Each tweet represents a list of (ID, word count) tuples. E.g., assuming the following mapping (word:ID): {im:0, feeling:1, so:2, happy:3, today:4, very:5}
  ```
  tweet ID,[(0, 1), (1, 1), (2, 2), (3, 2), (4, 1), (5,1) ]
  ```
  - tfidf: Same as “count” except that instead of word counts, tf-idf values are used, e.g.,
  ```
  tweet ID,[(0, 0.324), (1, 0.452), (2, 0.02), (3, 0.436), (4, 0.128), ... ]
  ```
  - glove100: Each word mapped to a 100-dimensional Glove “embedding vector” then the vectors of each word in a tweet summed to obtain a single 100-dimensional representation of the tweet, e.g.,
  ```
  tweet ID, [2.05549970e-02 8.67250003e-02 8.83460036e-02 -1.26217505e-01 1.31394998e-02, . . .]
  ```

  
