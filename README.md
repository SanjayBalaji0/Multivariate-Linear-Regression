# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Pandas Library.
### Step2
Read the csv file.

### Step3
Get values.

### Step4
Enter the parameters.

### Step5
Print the parameters.
## Program:
```
#Program to implement multivariate linear regression and predict the output.
#Developed by: S.Sanjay Balaji
#RegisterNumber: 23005804
import pandas as pd
from sklearn import linear_model

df = pd.read_csv("Multivalate Linear Regression.csv")
X=df[['Weight', 'Volume']]
Y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(X,Y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume', predictedCO2)





```
## Output:
![image](https://github.com/SanjayBalaji0/Multivariate-Linear-Regression/assets/145533553/badb8a65-ae8d-4749-9cc9-01b12332d867)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
