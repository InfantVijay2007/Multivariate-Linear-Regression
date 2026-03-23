# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Import the required libraries such as Pandas and Scikit-learn to handle data and perform linear regression.
### Step2
<br>
Read the cars.csv file using Pandas and store it in a dataframe.
### Step3
<br>
Select Weight and Volume as independent variables (X) and CO2 as the dependent variable (y).
### Step4
<br>
Create a linear regression model and train it using the dataset with the fit() function.
### Step5
<br>
Then use the trained model to predict the CO2 emission and display the result.
## Program:

# Developed by: Infant Vijay.A
# Register No: 212225240052
~~~
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
~~~
## Output:

<img width="1257" height="343" alt="567824802-8195d1db-6b4e-48a4-9307-f6ce4d92abbd" src="https://github.com/user-attachments/assets/319f2f47-9178-4462-94c1-01a6e865dcee" />

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
