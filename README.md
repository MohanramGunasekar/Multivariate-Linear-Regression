# Implementation of Multivariate Linear Regression
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
Get the value of X and y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
### Step 6:
Print the predicted output.


## Program:
```
# Developed by : Mohanram Gunasekar
# Register No : 212223240095

import pandas as pd
from sklearn import linear_model
data= pd.read_csv("cars.csv")

X=data[['Weight','Volume']]
Y=data['CO2']

regr=linear_model.LinearRegression()
regr.fit(X,Y)

print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)

predictCO2=regr.predict([[3300,1300]])
print("prediction CO2 for the corresponding weight and volume",predictCO2)





```
## Output:
![331243188-d151b51c-4385-4330-9c4f-e3c0612ec0f8](https://github.com/MohanramGunasekar/Multivariate-Linear-Regression/assets/139841812/9e797050-d57a-4aaa-8ade-553adaaf3981)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
