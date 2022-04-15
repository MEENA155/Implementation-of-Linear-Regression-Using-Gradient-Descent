# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to implement the linear regression using gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:
```
1.Use the standard libraries in python for Gradient Design.
2.Upload the dataset and check any null value using .isnull() function.
3.Declare the default values for linear regression.
4.Calculate the loss usinng Mean Square Error.
5.Predict the value of y.
6.Plot the graph respect to hours and scores using scatter plot function.
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
data = pd.read_csv("student_scores.csv")
data.head()
data.isnull().sum()
x = data.hours
x.head()
y = data.scores
y.head()
n= len(x)
m = 0
c = 0
L = 0.001
loss = []
for i in range(10000):
  Ypred = m*x+c
  MSE = (1/n) * sum((ypred -y)*2)
  dm = (2/m)* sum (x(Ypred - y))
  dc = (2/m)* sum (ypred - y)
  c = c-l*dc
  m = m-l*dm
  loss.append(MSE)
  #print(m)
print(m,c)
y_pred = m*x+c 
plt.scatter(x,y,color ='black')
plt.plot(x,y_pred)
plt.Xlable("study hours")
plt.ylable("score")
plt.title("study hours vs scores")
plt.plot(loss)
plt.xlable("iteration")
plt.ylable("loss")
*/
```

## Output:
![Screenshot (30)](https://user-images.githubusercontent.com/94677128/163543296-af66540f-6b43-4c33-a9f6-3b85fbde3f33.png)
![Screenshot (31)](https://user-images.githubusercontent.com/94677128/163543421-0ce4e471-4810-4741-92dd-890994bc8936.png)




## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
