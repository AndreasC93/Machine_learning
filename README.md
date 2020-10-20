# Machine_learning_hw
## credit_risk_resampling
1. Load the Lending Club data, split the data into training and testing sets, and scale the features data.
2. Oversample the data using the `Naive Random Oversampler` and `SMOTE` algorithms.
3. Undersample the data using the `Cluster Centroids` algorithm.
4. Over- and under-sample using a combination `SMOTEENN` algorithm.

For each of the above, you will need to:

1. Train a `logistic regression classifier` from `sklearn.linear_model` using the resampled data.
2. Calculate the `balanced accuracy score` from `sklearn.metrics`.
3. Calculate the `confusion matrix` from `sklearn.metrics`.
4. Print the `imbalanced classification report` from `imblearn.metrics`.

Questions/Answers
1. Which model had the best balanced accuracy score?
   Naive oversampling: 0.6550777362808256, SMOTE oversampling: 0.642860308366672, Undersampling: 0.519883284785928, Combination sampling: 0.6162891652666482. Based on these accuracy scores the naive oversampling model had the highest accuracy score at approx 0.655
2. Which model had the best recall score?
   Naive oversampling: 0.65, SMOTE oversampling:  0.66, Undersampling:  0.41, Combination sampling: 0.53. Based on these average recall scores the SMOTE model had the best recall score.
3. Which model had the best geometric mean score?
   Naive oversampling:  0.66, SMOTE oversampling:  0.64, Undersampling:  0.51, Combination sampling: 0.64. Based on these geometric mean scores the naive oversampling model had the best score.
## credit_risk_ensemble
1. Load the Lending Club data, split the data into training and testing sets, and scale the features data.
2. Train the model using the quarterly data from LendingClub provided in the `Resource` folder.
3. Calculate the balanced accuracy score from `sklearn.metrics`.
4. Print the confusion matrix from `sklearn.metrics`.
5. Generate a classification report using the `imbalanced_classification_report` from imbalanced learn.
6. For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.

Questions/Answers

1. Which model had the best balanced accuracy score?
   Random Forest Classifier: 0.6569659094662335, Easy Ensemble Classifier: 0.6994564899809197. Based on these accuracy scores the Easy Ensemble model had the best balanced accuracy score 0.6994564899809197.
2. Which model had the best recall score?
   Random Forest Classifier:  1.00, Easy Ensemble Classifier: 0.80. Based on these recall scores the Random Forest model had the best recall score 1.00.
3. Which model had the best geometric mean score?
   Random Forest Classifier:  0.56, Easy Ensemble Classifier: 0.69. Based on these geometric mean scores the Easy Ensemble model had the best score 0.69.
4. What are the top three features?
   The top three features are: (0.08301006201890893, 'total_pymnt'), (0.07945232463258912, 'out_prncp_inv'), (0.07749574978451985, 'total_rec_late_fee').
