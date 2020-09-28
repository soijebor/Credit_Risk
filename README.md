# Credit_Risk

## ***Project Overview***

  * Explain how a machine learning algorithm is used in data analytics.
  * Create training and test groups from a given data set.
  * Implement the logistic regression, decision tree, random forest, and support vector machine algorithms.
  * Interpret the results of the logistic regression, decision tree, random forest, and support vector machine algorithms.
  * Compare the advantages and disadvantages of each supervised learning algorithm.
  * Determine which supervised learning algorithm is best used for a given data set or scenario.
  * Use ensemble and resampling techniques to improve model performance.
  
## ***Resources***
  
  * Data Source: LoanStats_2019Q1.csv
  * Software: Python 3.7.6, Anaconda 4.8.4, Jupyter Notebook 6.0.3
  
## ***Challenge Overview***
  
Credit risk is an inherently unbalanced classification problem, as the number of good loans easily outnumber the number of risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Your final task is to evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

  * Oversample the data using the RandomOverSampler and SMOTE algorithms.
  * Undersample the data using the cluster centroids algorithm.
  * Use a combination approach with the SMOTEENN algorithm.

For each of the above:

  * Train a logistic regression classifier (from Scikit-learn) using the resampled data.
  * Calculate the balanced accuracy score using balanced_accuracy_score from sklearn.metrics.
  * Generate a confusion_matrix.
  * Print the classification report (classification_report_imbalanced from imblearn.metrics).

### ***Challenge Extension***
* Use 100 estimators for both classifiers, and complete the following steps for each model:
  * Train the model and generate predictions.
  * Calculate the balanced accuracy score.
  * Generate a confusion matrix.
  * Print the classification report (classification_report_imbalanced from imblearn.metrics).
  * For the BalancedRandomForestClassifier, print the feature importance, sorted in descending order (from most to least important feature), along with the feature score.


### ***Challenge Summary***

* #### ***Naive Random Oversampling***

For the Naive Random Oversampling algorithm,I resampled the training data with the RandomOversampler. I got a count of 'low_risk': 51366, 'high_risk': 51366. I used the resampled data to train the Logistic Regression model. The precision and recall average scores were 0.99 and 0.55 respectively with the balanced accuracy score of 0.65. 


* #### ***SMOTE Oversampling***

For the SMOTE Oversampling algorithm,I resampled the training data with SMOTE. I got a count of 'low_risk': 51366, 'high_risk': 51366. I used the resampled data to train the Logistic Regression model. The precision and recall average scores were 0.99 and 0.69 respectively with the balanced accuracy score 0.66. 

* #### ***Undersampling***

For the Undersampling algorithm,I resampled the training data with ClusterCentroids resampler. I got a count of 'high_risk': 246, 'low_risk': 246. I used the resampled data to train the Logistic Regression model. The precision and recall average scores were 0.99 and 0.42 respectively with the balanced accuracy score 0.54.

* #### ***Combination (Over and Under) Sampling***

For the Combination (Over and Under) Sampling algorithm,I resampled the training data with SMOTEENN. I got a count of 'high_risk': 51361, 'low_risk': 46653. I used the resampled data to train the Logistic Regression model. The precision and recall average scores were 0.99 and 0.58 respectively with the balanced accuracy score 0.64.

In conclusion, from the four methods used the SMOTE Oversampling had the highest recall score of 0.69 while Undersampling had the lowest recall score of 0.42. For the balanced accuracy score, the SMOTE Oversampling algorithm had the highest. Although all the algorithms show poor predicting results, I will recommend the SMOTE Oversampling since it is giving the most balanced result but I recommend an increases Logistic Regression Model by using a higher max_iter of at least 200.

### ***Extension Summary***

* #### ***Balanced Random Forest Classifier***

For the Balanced Random Forest Classifier algorithm,I resampled the training data with RandomOversampler. The precision and recall average scores were 0.99 and 0.87 respectively with the balanced accuracy score 0.79.

* #### ***Easy Ensemble AdaBoost Classifier***

For the Easy Ensemble AdaBoost Classifier algorithm,I resampled the training data with RandomOversampler. The precision and recall average scores were 0.99 and 0.94 respectively with the balanced accuracy score 0.93.
