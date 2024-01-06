# ML-for-Texts-Film-Sentiment-Analysis
Sentiment Analysis in Classic Movie Reviews: Building a Predictive Model for The Film Union

## Project Description
The Film Now Union, a new edgy community for classic movie enthusiasts, is developing a system for filtering and categorizing movie reviews. The goal is to train a model to automatically detect negative reviews. You'll be using a dataset of IMBD movie reviews with polarity labelling to build a model for classifying positive and negative reviews. It will need to have an F1 score of at least 0.85.

## Data Description
The data is stored in the imdb_reviews.tsv file. 

The data was provided by Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts. (2011). Learning Word Vectors for Sentiment Analysis. The 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011).

Description of the selected fields:
review: the review text
pos: the target, '0' for negative and '1' for positive
ds_part: 'train'/'test' for the train/test part of dataset, correspondingly.

## Conclusion

**Performance against Baseline (Model 0):** Model 4, like the other models, is significantly better than the baseline Model 0 in every aspect. It demonstrates the value of complex models over a simple constant baseline.

**Comparison with Models 1 and 3:** Model 4 has a slightly lower accuracy (0.86) compared to Models 1 and 3 (0.90). This might be due to the differences in the underlying algorithms (LGBM vs. Logistic Regression). The precision, recall, and F1 scores are also slightly lower but still reflect a strong model performance.

**Model Characteristics:** The use of LightGBM might offer advantages in terms of training speed and handling large datasets, despite a slight drop in performance metrics. This trade-off could be beneficial in certain applications where scalability and speed are more critical.

**Performance of Model 4:** This model showcases the application of a gradient boosting framework in text classification tasks, providing a competitive alternative to logistic regression-based models. While it slightly underperforms in accuracy compared to Models 1 and 3, it still greatly surpasses the baseline and may offer practical advantages in specific scenarios. The choice between logistic regression and gradient boosting models would depend on the specific requirements of the task, such as the need for speed and scalability versus the highest possible accuracy.
