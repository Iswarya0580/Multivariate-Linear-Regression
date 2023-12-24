# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1
Import panda

### Step 2
Import linear model from sklearn

### Step 3
Read the file cars.csv

### Step 4
Assign the values for x and y as required

### Step 5
Create the linearRegression model and predict the output


## Program:
```
#DEVELOPED BY: Iswarya.P
#REG NO: 23013459

import pandas as pd
from sklearn import linear_model
df =pd.read_csv("cars(1).csv")
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
![Alt text](multiline-1.png)

### Insert your output
![Alt text](<Screenshot 2023-12-24 113244-1.png>)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.