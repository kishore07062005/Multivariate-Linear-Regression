# Ex-10: Implementation of Multivariate Linear Regression
### DATE: 
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.
### Step2
Read the csv file.

### Step3
Get the value of X and y variables

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 3300kg, and the volume is 1300cm cube.

## Program:
```
#Developed By: KISHORE.M
#Register Number: 2305002012

import pandas as pd
from sklearn import linear_model
data=pd.read_csv("car.csv")
x=data[["Weight","Volume"]]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficients:",regr.coef_)
print("Intercept:",regr.intercept_)
predCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predCO2)
```
## Output:
![WhatsApp Image 2024-05-24 at 21 19 14_bb92f98d](https://github.com/kishore07062005/Multivariate-Linear-Regression/assets/156066116/c65f9841-7a9b-4762-9e11-10d58da01609)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
