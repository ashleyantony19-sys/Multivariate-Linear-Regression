# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step 1

Import the required libraries such as NumPy, Pandas, and LinearRegression from sklearn.

Step 2

Load or create the dataset containing multiple input features and the target output.

Step 3

Separate the dataset into independent variables (X) and dependent variable (y).

Step 4

Create and train the Multivariate Linear Regression model using the training data.

Step 5

Predict the output using the trained model and display the predicted result.

## Program:
```

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))


```
## Output:

<img width="327" height="97" alt="Screenshot 2026-05-19 215201" src="https://github.com/user-attachments/assets/827e065e-135c-42f6-822b-1d1fdeb9c70f" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
