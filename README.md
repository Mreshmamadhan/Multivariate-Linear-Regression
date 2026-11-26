# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:Implementation of Multivariate Linear Regression

### Step1
<br>Start the program and import the required libraries such as NumPy, Pandas, and Scikit-learn.
### Step2
<br>Load the dataset and separate the independent variables (X) and dependent variable (Y).
### Step3
<br> Split the dataset into training and testing data using the train_test_split() function.
### Step4
<br>Create and train the Multivariate Linear Regression model using the LinearRegression() function and fit() method.
### Step5
<br>Predict the output using the predict() method and display the predicted results.
## Program:
```
# Developed by: Reshma M
# ref No.:26018352
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)

```
## Output:

### Insert your output

<br><img width="1920" height="1080" alt="Screenshot (49)" src="https://github.com/user-attachments/assets/689ce7eb-2b2f-4e68-9963-af789990b086" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
