# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas.

### Step2
Import linear_modal from sklearn.

### Step3
Read the file using read_csv.

### Step4
Get the inputs from the user as x and y.

### Step5
Use regr.fit(x,y) to et the output.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight', 'Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients: ', regr.coef_)
print('Intercept:', regr.intercept_)
predictedCO2=regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume:',predictedCO2)
```
## Output:
### Insert your output

<img width="561" alt="2022-02-17 (3)" src="https://user-images.githubusercontent.com/94505585/154455937-ab23d51b-9d5f-4b12-a422-7d3836499c03.png">


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
