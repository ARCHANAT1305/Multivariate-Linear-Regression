# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step1
Import the necessary libraries, pandas and scikit-learn, and loads the dataset 'cars.csv.txt' into a DataFrame named df.

### Step2
create two DataFrames, a and b, representing the input features ('Weight' and 'Volume') and the output variable ('CO2').
### Step3
Initializes a linear regression model (regr) and trains it using the input features (a) and the output variable (b).
### Step4
print the coefficients and intercept of the trained linear regression model.
### Step5
Make a prediction using the trained model for a new input of 'Weight=3300' and 'Volume=1300' and prints the predicted 'CO2' emissions.
## Program:
```
Developed By: ARCHANA.T
Register No: 212223240013

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('cars.csv.txt')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("coefficient ",regr.coef_)
print("Intercept: ",regr.intercept_)
print("Amount: ",regr.predict([[3300,1300]]))
```
## Output:
![cars csv](https://github.com/ARCHANAT1305/Multivariate-Linear-Regression/assets/145975189/a50c48cd-bb7d-494b-806c-f0fce76ef450)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
