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
#Developed By: Rahul M R
#Register Number: 2305003005

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
![image](https://github.com/RahulM2005R/Multivariate-Linear-Regression/assets/166299886/933fee9f-8a94-4f96-901f-219f62b480e8)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
