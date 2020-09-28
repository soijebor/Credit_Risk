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
  
  * Implement machine learning models.
  * Use resampling to attempt to address class imbalance.
  * Evaluate the performance of machine learning models.
  
***
  * Oversample the data using the RandomOverSampler and SMOTE algorithms.
  * Undersample the data using the cluster centroids algorithm.
  * Use a combination approach with the SMOTEENN algorithm.

For each of the above, you’ll:

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


## ***Challenge Summary***
