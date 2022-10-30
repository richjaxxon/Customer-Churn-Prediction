# Customer-Churn-Prediction

Customer churn is an issue most businesses face, particularly those that employ a subscription service. Companies need to know the factors that contribute to customer churn and make plans to stop customers from leaving before they do so. The primary goal of this exercise is to build a machine-learning model that can predict customer churn based on the given information in the dataset.

## Data

The dataset comes from an IBM development platform for a fictitious phone/internet company called Telco. It can be accessed through IBM and is available on Kaggle as well. The dataset has 21 columns and 7043 rows of data which has information on 5174 current customers and 1869 customers who have churned. 

## Exploratory Data Analysis

When looking at the data, some of the relationships which can be determined are:
Customers with no online security or backup, no device protection, and no tech support are from two to three times more likely to churn. Customers with month-to-month contracts are almost four times more likely to churn than customers with yearly contracts. Two-year contractors are very unlikely to churn.

## Modeling
I first used a Logistic Regression model using Scikit-Learn. I then built a Random Forest Classifier model, which had slightly better recall than Logistic regression but had less precision and less accuracy than the Logistic Regression model.
I used a Grid search CV to find the optimal parameters for the Random Forest Model. After putting in the new parameters I was able to increase the accuracy of the Random Forest Model. 

## Final Results
Even though hyper tuning increased the Random Forest Model slightly, the logistic regression model still performed better and is the model I would use.
