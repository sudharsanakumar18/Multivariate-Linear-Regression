# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import panda

### Step2
Import linear model from sklearn

### Step3
Read the file cars.csv

### Step4
Assign the values for x and y as required

### Step5
Create the linearRegression model and predict the output

## Program:
```
#DEVELOPED BY: SUDHARSANA KUMAR S R
#REG NO: 23007374
import pandas as pd
from sklearn import linear_model
df =pd.read_csv("cars.csv")
x= df[["Weight","Volume"]]
y= df["CO2"]
regr =linear_model.LinearRegression()
regr.fit(x,y)
print("coefficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedco2=regr.predict([[3000,1200]])
print("Predicted co2 for the coressponding weight and volume ",predictedco2)
```
## Output:
![mat ai 10](https://github.com/sudharsanakumar18/Multivariate-Linear-Regression/assets/138849110/c104460d-3978-4462-b40b-88efb70ced7b)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
