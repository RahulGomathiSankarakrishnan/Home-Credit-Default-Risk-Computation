# The project is based on the Home Credit Default Risk (HCDR) Kaggle Competition. The goal of this project is to predict whether or not a client will repay a loan. In order to make sure that people who struggle to get loans due to insufficient or non-existent credit histories have a positive loan experience, Home Credit makes use of a variety of alternative data--including telco and transactional information--to predict their clients' repayment abilities.

# Abstract
Home Credit Default Risk Computation is a project where we determine the credit worthiness of people that have applied for the loans. In previous phases, we had completed basic EDA, Feature Engineering and ran the baseline model for logistic regression and the hyperparameter tuning for XGBoost model. In Phase 2, we have significantly improved our project. We have updated the EDA, implemented robust Feature engineering for all dataset files, and did experimental analysis for hyper-parameter tuning for Logistic Regression, XGBoost and Random Forest Models. We conducted experiments using both original imbalanced data as well as resampled data. After comparison we found out that the XGBoost model was the best model. For the deep learning Pytorch model, we built two MLP models. One for classification and one for regression. The mail goal in this phase has been building a multi-layer perception (MLP) model in PyTorch for loan default classification and using Tensorboard to visualize the results of training in real time. Each model has 3 layers. Sigmoid activation function is used for classification and ReLU for regression along with Cross entropy loss. We have acheived a Test accuracy of 92 and Test CXE loss of 0.29.

# Project Description and Data
Data Description
Many people struggle to get loans due to insufficient or non-existent credit histories. And, unfortunately, this population is often taken advantage of by untrustworthy lenders. Home Credit strives to broaden financial inclusion for the unbanked population by providing a positive and safe borrowing experience. In order to make sure this underserved population has a positive loan experience, Home Credit makes use of a variety of alternative data--including telco and transactional information--to predict their clients' repayment abilities. Various statistical and machine learning methods can be used to make these predictions.

# Data Files Overview:
There are 7 different sources of data:

application_train/application_test: the main training and testing data with information about each loan application at Home Credit. Every loan has its own row and is identified by the feature SK_ID_CURR. The training application data comes with the TARGET indicating 0: the loan was repaid or 1: the loan was not repaid. The target variable defines if the client had payment difficulties meaning he/she had late payment more than X days on at least one of the first Y installments of the loan. Such case is marked as 1 while other all other cases as 0.
bureau: data concerning client's previous credits from other financial institutions. Each previous credit has its own row in bureau, but one loan in the application data can have multiple previous credits.
bureau_balance: monthly data about the previous credits in bureau. Each row is one month of a previous credit, and a single previous credit can have multiple rows, one for each month of the credit length.
previous_application: previous applications for loans at Home Credit of clients who have loans in the application data. Each current loan in the application data can have multiple previous loans. Each previous application has one row and is identified by the feature SK_ID_PREV.
POS_CASH_BALANCE: monthly data about previous point of sale or cash loans clients have had with Home Credit. Each row is one month of a previous point of sale or cash loan, and a single previous loan can have many rows.
credit_card_balance: monthly data about previous credit cards clients have had with Home Credit. Each row is one month of a credit card balance, and a single credit card can have many rows.
installments_payment: payment history for previous loans at Home Credit. There is one row for every made payment and one row for every missed payment.

# Tasks Performed in each phase
## Phase 1
EDA and Building a baseline pipeline model

## Phase 2
Feature Engineering and Hyperparameter tuning, Feature Selection ensemble methods

## Phase 3
Build a multi-layer perception (MLP) model in PyTorch for loan default classification Using Tensorboard to visualise the results of training in real time
