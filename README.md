
# Classification of Congressional Voting Records using Random Forest
    1. Project Motivation
    2. Objectives
    3. Methods Used
    4. Installation
    5. Data
    6. Implementation
    7. Result


## 1. Project Motivation

In the ***House of Representatives***, the *majority party* holds significant power to draft chamber rules and schedule bills to reach the floor for debate and voting. Every year 100's of bills are passed by the congress which are enacted into the law. While many laws are enacted, it isn't easy for every law to pass thru without significant effort by both the parties either to support or oppose it. Bills contain elements which are ***both oppposed and supposed by the members of both majority and minority group owing to the local sentiments***.

Hence, a machine learning model encompassing various bills across many agendas might ***help the legislator to prioritise which points to give importance in their legislation***. 

## 2. Objectives
* Obtain the dataset from UCI Repository
* Find appropriate features and transform them for classification
* Find the best possible Hyperparameters for the model
* Perform Cross-Validation on the best model
* Visualize the Tree and find the importance of each feature
## 3 Methods Used
* Feature Engineering
* Using RandomizedSearchCV for best Hyperparameters
* Random Forest Classifier
## 3 Methods Used
* Feature Engineering
* Using RandomizedSearchCV for best Hyperparameters
* Random Forest Classifier
## 4 Installation
* Python versions 3.*.
* Python Libraries:
    * Pandas
    * Numpy
    * Sklearn
* Graphviz
* Ipython
## 5. Data
The data is loaded from .data file downloaded from UCI repository. The dataset has about ***16 bills as features*** and ***400 members as rows***.
## 6. Implementation
I have selected all ***16 bills as features*** for the model and ***Party is taken as target variable***.

The features have ***y,n and ?*** which are ***categorical*** in nature. They are converted into numeric type for classsification.

The target variable has only 2 categories: ***democrat or republican***. They have been converted into numeric type data too.

***Hyperparameters*** are varied for ***'n_estimators' and 'max_depth'*** for best model fit. ***Cross Validation*** has been performed on the best fitting model. Prediction is done and ***performance metrics*** are found. 
## 7. Result
The dataset has been classified using a ***Random Forest Classifier***. ***Decision Tree*** and ***feature importance*** has been visualized.