# Study of maximizing loan profits
Analysis and preprocessing of high dimensional unbalanced data set

## Library
Install imblearn by using the command : `pip install imblearn`

## Project Background
For the business of bank lending, we simplify the analytical model. 

After the bank provides a loan, if the lender has the ability to repay, the bank will receive interest as profit. And if the lender is unable to repay, we simply assume that the bank will lose that money.

Therefore, in order to maximize profits, banks should, as far as possible, lend money to those who can actually repay it and avoid giving it to those who actually cannot.
Statistically speaking, that is, to increase *True Positive Rate* and decrease *False Positive Rate*.

In real life, however, the distribution of data is not always balanced. For example, people who have cancer, people who win the lottery, they are always a minority of the population. When training the model,if we use unbalanced data,  we may get high accuracy, however other indicators may be very unsatisfactory (e.g. a very high False Positive Rate)

Therefore, in this case, we focus on exploring how to handle unbalanced data.


## File Description
1. *LoanStats3a.zip* : Original data set. Unfortunately, the website of the data source no longer exists and it is difficult to find the explanation of the meaning of some features.
2. *Maximize loan profit.ipynb* : Project code file. The notebook is exploratory in searching for data related to the problem shown in the notebook title. Markdown cells are used to help complete the various steps in the thinking process.


## Key Points
1. Use the parameter `class_weight` that come with the machine learning model of sklearn 
2. Use the *oversampling* or *undersampling* method to balance the data.

## Result
Reduced the false positive rate from 90% to 7%, while the recall drops from 98% to 61%
