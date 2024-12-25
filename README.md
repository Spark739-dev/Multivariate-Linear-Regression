# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br> Import pandas as pd and sklearn into that import linear_model, by importing pandas and sklearn from python library.

### Step2
<br>use pandas inbuilt function to get and input csv file from user using pd.read_csv(path of csv file) command.

### Step3
<br>From dataset select dependent variable and one independent variable to and to find the relationship of one more two independent variables.

### Step4
<br>use linearmodel into that use linear regression function to computr the variables.

### Step5
<br>use regression.fit function of inputted variables of x and y and print corresponding results to get output.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("C:\\Users\\admin\\Downloads\\car.csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print("Coefficient",regression.coef_)
print("Intercept",regression.intercept_)
print("CO2 required is",regression.predict([[100,929]]))






```
## Output:
![output](output.png)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.