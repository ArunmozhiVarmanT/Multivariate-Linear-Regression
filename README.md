# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step1

Import pandas as pd.
### Step2
Read the csv file.

### Step3
Get the value of X and y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
### Program for Implementation of Multivariate Linear Regression
### Developed by: ARUNMOZHI VARMAN T
### Register Number:2122223230022
```
from sklearn import linear_model
df = pd.read_csv("cars.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
print('Amount:',regr.predict([[3300, 1300]]))
```
## Output:
![image](https://github.com/ArunmozhiVarmanT/Multivariate-Linear-Regression/assets/144870523/56946056-a1fe-4884-91f1-7d53109b6071)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
