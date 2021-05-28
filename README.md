# Graph-based Explanations
This repository contains the implementation of graphs-based models to generate explanations using link prediction techniques. These models are useful when we need to explain recommendations from black-box recommender systems. 
The folders we have in this repository are:
- **analysis_dataset** contains the notebook we used to analyse the MovieLens 100K dataset, which is the dataset we have employed to evaluate our model.
- **original_evaluation** contains the notebooks to implement the "original" evaluation of our graph-based methods. In this evaluation, we built the graph-based model with 90% of the interactions. The remaining 10% of the interactions are used to build the test set. We have two notebooks, one for the building and the evaluation of the item-based model, and the other to build and evaluate the user-based model.
- **stratified_evaluation** contains the notebooks to implement the "stratified" evaluation of our graph-based methods. In this case, we evaluate the models having the same number of interactions for each rating value in the test set to delete the original evaluation's bias. We also have two different models: an item-based method and a user-based model.

In these folders, we have the datasets to run the notebooks too. They are the following datasets:
- **trainset.csv** is the file with 90% of the dataset to build the training set. We have used it in both original and stratified evaluations.
- **predicted_values.csv** is the test set used in the evaluation. It contains the ratings predicted by the matrix factorisation recommender system used in the evaluation.
- **testset_stratified.csv** is the test set used in the stratified evaluation. We have used in combination with predicted_values.csv to carry out the stratified evaluation.


