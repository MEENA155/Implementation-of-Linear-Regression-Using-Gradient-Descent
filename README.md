# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to implement the linear regression using gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:
```
1.Import the standard Libraries.
2.Set variables for assigning dataset values.
3.Import linear regression from sklearn.
4.Assign the points for representing in the graph
5.Predict the regression for marks by using the representation of the graph.
6.Compare the graphs and hence we obtained the linear regression for the given datas.
```

## Program:
```
/*
Program to implement the linear regression using gradient descent.
Developed by: S.Meena
RegisterNumber:  212221240028
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
dataset = pd.read_csv('student_scores.csv')
dataset.head()
X=dataset.iloc[:,:-1].values
Y=dataset.iloc[:,1].values
from sklearn.model_selection import train_test_split
X_train,X_test,Y_train,Y_test = train_test_split(X,Y,test_size = 1/3,random_state = 0)
from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
regressor.fit(X_train,Y_train)
Y_pred = regressor.predict(X_test)
plt.scatter(X_train,Y_train,color="purple")
plt.plot(X_train,regressor.predict(X_train),color="green")
plt.title("Hours vs Scores (Training Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
plt.scatter(X_test,Y_test,color="brown")
plt.plot(X_train,regressor.predict(X_train),color="blue") 
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
*/
```

## Output:
![Screenshot (17)](https://user-images.githubusercontent.com/94677128/162006790-e3eb2859-6e34-4ac0-b4b4-c82da12f2ddd.png)
![Screenshot (18)](https://user-images.githubusercontent.com/94677128/162006996-b34573b3-ab34-4b0e-851f-295923bb3238.png)



## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
