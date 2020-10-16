# Sentence-Inference
For every given pair of sentences -- (sentence-1, sentence-2), we need to determine if sentence-2 can be logically inferred given sentence-1.

## Dataset Description:
* `Sentence1`: String column of human entered text, Sentence 1
* `Sentence2`: String column of human entered text, Sentence 2
* `gold_label`: Categorical column inferring logical relation between sentence1 and sentence2

## Implementation 
* Length of document in sentence1: 
![Length of strings Sentence1](https://github.com/paras009/Sentence-Inference/blob/master/images/length_of_doc_s1.png)
* Length of document in sentence2: 
![Length of strings Sentence2](https://github.com/paras009/Sentence-Inference/blob/master/images/length_of_doc_s2.png)
* Heatmap of correlation between the features: 
![Heatmap](https://github.com/paras009/Sentence-Inference/blob/master/images/correlation_heatmap.png)
* Bidirectional LSTM Model performance(not good due to less data): 
![Loss](https://github.com/paras009/Sentence-Inference/blob/master/images/bidirectional_LSTM_model_performance_loss.png)
![Accuracy](https://github.com/paras009/Sentence-Inference/blob/master/images/bidirectional_LSTM_model_performance_accuracy.png)
* Selected model's performance for predicting the testing `gold_label`.
![MLPClassifier](https://github.com/paras009/Sentence-Inference/blob/master/images/MLPClassifier.PNG)

## Inference
* Since the dataset was very small, training a Neural network was not a good idea so I choose to move ahead with ML algorithms. 
* So, working on a large dataset can improve the learning.
* Advanced NLP techniques can be implemented to find the semantic relationship between both the sentences to get a better result.
* Due to lack of time I decided to follow this approach but with various iterations during the development, model's performance can increase significantly.
* `Data Cleaning` was done signifantly well but can be done using other approaches.
* `Feature engineering` is one important part which require good knowledge of NLP which can be worked upon in future.
* Dimensionality reduction based on experimentation on using `PCA` or `t-SNE` can be perfromed to optimize model performance and remove useless features.
* `Hypothesis testing` can be done in making useful decissions about the feature, whether they contribute in predicting right `gold_label` or not.
* `Word ebedding` can be implemented to get a better semantic relationship between words.
* Working with more better Neural Networks will be a better choice for this kind of problem, although `bidirectional LSTM` should perform well with large dataset.
* Finally once we get a good model performance over the data, we can implement hyperparameter tuning to tune those small knobs in the `bidirectional LSTM` model to extract the best performance out of it.
* for any suggestions contact me at [sanjoy.eee32@gmail.com](sanjoy.eee32@gmail.com)
