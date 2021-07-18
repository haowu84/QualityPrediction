# WineQuality

## Abstract
In this assignment, different classification techniques are investigated to predict the quality of red and white vinho verde samples from Portugal. The chemical elements of wine are used to classify the quality. Data preprocessing and hyperparameter tuning are also performed to achieve the optimal performance.

## Data Exploration/Preprocessing
The data distributions of some features are skewed. To remove long tails and possible outliers, the data needs to be transformed into Gaussian distributions with zero mean and unit variance.

## Feature Selection
The dataset has 11 features in total, but only a few features contribute to the quality. The feature importance is calculated based on the number of splits that include the feature in a random forest model (gini importance). Feature selection methods need to be applied. Cross validation is used to select the optimal number of features.

## Model Exploration/Performance Validation
All data will be trained and tested with 5-fold cross validation.

### LogisticRegression
c: the regularization strength

### Support Vector Machine 
c: the penalty for misclassified data points  
gamma: the distance of influences that data points have on the decision boundary  
kernel: the function that transforms the data to higher dimensional space  

### KNN
n_neighbors: the number of neighbors to use   
weight: weight function on distance

### Decision Tree/Random Forest 
max_depth: the maximum depth of each decision tree  
min_samples_split: the minimum amount of data points required before a node can be split  
min_samples_leaf: the minimum amount of data points allowed in a leaf node  

### Ada Boost
learning_rate: contribution of each classifier  
n_estimators: number of estimators   
