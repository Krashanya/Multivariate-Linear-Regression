# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
1.Import necessary libraries (e.g., NumPy, Pandas, Scikit-learn) 2.Load your dataset into a Pandas DataFrame
<br>

### Step2
1.Handle missing values (e.g., imputation, removal) 2.Scale/normalize features (e.g., StandardScaler)
<br>

### Step3
1.Split data into training (~70-80%) and testing sets (~20-30%) 2.Create a Multivariate Linear Regression
model (e.g., Scikit-learn's LinearRegression)
<br>

### Step4
1.Fit the model to the training data 2.Evaluate the model using metrics like MSE, R-squared, and MAE
<br>

### Step5
1.Refine the model by tuning hyperparameters or feature engineering 2.Deploy the final model in your
desired application or platform
<br>

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("C:\\Users\\admin\\Downloads\\car.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)






```
## Output:

###
<img width="730" height="142" alt="image" src="https://github.com/user-attachments/assets/f7d1a5ae-1a9b-48d0-95e6-2c590406e07c" />


<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
