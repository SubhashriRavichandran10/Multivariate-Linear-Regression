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
#DEVELOPED BY: R.SUBHASHRI
#REG NO:23012776

import pandas as pd
from sklearn import linear_model

df = pd.read_csv('employee.csv')

x = df[['Experience', 'Education']]
y = df['Salary']

regr = linear_model.LinearRegression()
regr.fit(x, y)

print("Coefficient:", regr.coef_)
print("Intercept:", regr.intercept_)

new_employee = [[5, 2]]  
predicted_salary = regr.predict(new_employee)

print("Predicted Salary for the corresponding experience and education:", predicted_salary)





```
## Output:

![Screenshot 2024-01-02 233507](https://github.com/SubhashriRavichandran10/Multivariate-Linear-Regression/assets/145743413/49635ad2-08ed-48b3-81f1-ceaf45de1737)

![Screenshot 2024-01-02 233520](https://github.com/SubhashriRavichandran10/Multivariate-Linear-Regression/assets/145743413/5c9cf7df-6f96-4163-86b6-70c9fa857f4d)


![Screenshot 2024-01-02 233526](https://github.com/SubhashriRavichandran10/Multivariate-Linear-Regression/assets/145743413/8891f402-4909-4a0b-b1ef-7cad9fb9776f)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
