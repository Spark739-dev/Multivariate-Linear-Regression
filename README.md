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
<br>Use pandas inbuilt function to get and input csv file from user using pd.read_csv(path of csv file) command.

### Step3
<br>From dataset select a two one independent variable is (Volume) and another is independent variable(Weight)  and one dependent  variable (CO2) to and to find the relationship of one  or more two variables.

### Step4
<br>Use linearmodel into that use linear regression function to compute the variables.

### Step5
<br>Use regression.fit function of inputted variables of x and y and print corresponding results to get output.

### Step6
<br>Print Coefficient with use inbuilt function of regression(regression.coef_).

### Step7
<br>Print intercept with use of inbuilt function of regression(regression.intercept_).

### Step8
<br>Print CO2 required using inbuilt function of regression(regression.predict([100,929])). 
## Program:
```
Developed by:Veshwanth
Regno:24010033



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