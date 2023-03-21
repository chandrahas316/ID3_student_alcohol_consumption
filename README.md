# Student-Alcohol-Consumption-Analysis-EDA-and-Decision-Tree-ID3-Model

## Theory 

- For data preprocessing we need to do three things,

  1\. Finding correlation between variables so that highly correlated variables can be removed to reduce the redundancy in the dataset.

  ➔ We used pearson correlation method for numeric data and for the rest we used chi-square correlation method.

  2\. Checking whether there are any missing values in the dataset.

  ➔ There are no missing values in the given dataset.

  3\. Removing outliers in dataset.

- Decision tree(ID3) -

  ➔ We use decision tree to make a decision that is to predict the class.Each node(other than leaf nodes) is used to make the decision and leaf nodes represent the outcome of the test data.

  ➔ Id3 algorithm is used to get the decision tree of the dataset.

  ➔ In Id3 algorithm,We use Information gain to find the best possible splitting feature.

  ➔ Now split the dataset using the feature with max information gain and if all rows belong to the same class,make the current node as leaf node with the class as its label.Repeat this for the remaining features until we run out of all features or the tree has all leaf nodes.

- Bootstrap sampling method -

  ➔ It estimates the sampling distribution by taking multiple samples with replacement from a single random sample.This is done repeatedly and we will find the average of all the accuracy of samples.


- K - fold cross validation -

  ➔ In this we take k number of folds(mostly 5/10) and one will be the test set and the rest will be training set.

  ➔ We will apply the model repeatedly for k times because we need to take every fold as test set for once.

  ➔ Now we can calculate statistics like accuracy etc.., in each iteration and we will take average of all the iterations.we will decide the best k value based on the maximum statistics.

- Performance measures -

  ➔ Confusion matrix - It is a matrix of size 2X2 with actual values on one axis and predicted values on the other axis. Lets say,

  TN - true negative(both actual and predicted are negative)

  TP - true positive(both actual and predicted are positive)

  FP - false positive (Actually positive but incorrectly classified as negative)

  FN - false negative(Actually negative but incorrectly classified as positive)

  ➔ Accuracy : Number of instances that are correctly classified i.e..,

  Accuracy = (TP+TN)/total

  ➔ Precision:out of + predicted, number of instances that are actually -

  Precision = TP/(TP+FP)

  ➔ Recall:out of actually + ,number of instances that are + predicted.

  Recall = TP/(TP+FN)

  ➔ F1 score: Harmonic mean of precision and recall.

  F1 score = 2\*Precision\*Recall/(Precision+Recall)


## Code implementation 

- Installing and loading all the required libraries.

- Data Preprocessing

- Data Analysis 

- Implementing Decision tree using ID3 algorithm

- Performance metrics
