#Sentence Inference
In this problem, there are two files, `train.csv` and `test.csv`. 

In `train.csv`, the columns are `gold_label`, `sentence1` and `sentence2`. The gold label represents of whether the events talked about in the two sentences can 

- occour together or have `entailment`, 

- or if they contrdict each other or are `contradiction`

- or if they are unrelated to each other `neutral`

Your task is to build a model to predict these labels. 

After building the model, you will generate a predictions for the sentences in the `predicted.csv` file which will contain the predicted labels for the sentences in `test.csv`. These predicted labels must be in the same order as the sentences in `test.csv`.

A sample of the same is given as `test_sample.csv` and `predicted_sample.csv`.

You will submit `predicted.csv`.