## DATE:
# EX-10: Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:
import pandas as pd.

### Step2:
Read the csv file.

### Step3:
Get the value of X and y variables.

### Step4:
Create the linear regression model and fit.

### Step5:
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

### Step6:
Print the predicted output.

## Program:
```
print("Developed by: Harsshitha lakshmanan") 
print("RegisterNumber: 212223230075")

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients: ',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:
![image](https://github.com/user-attachments/assets/60b98eef-62ea-4639-b07f-52580b4fc14e)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
