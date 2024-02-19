# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the standard Libraries.
2.Set variables for assigning dataset values.
3.Import linear regression from sklearn.
4.Assign the points for representing in the graph.
5.Predict the regression for marks by using the representation of the graph.
6.Compare the graphs and hence we obtained the linear regression for the given datas. 

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Sanjay K
RegisterNumber: 212223220094
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from sklearn.metrics import mean_absolute_error,mean_squared_error
df=pd.read_csv("C:/Users/admin/Downloads/student_scores.csv")
df.head()
df.tail()
x=df.iloc[:,:-1].values
x
y=df.iloc[:,1].values
y
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=1/3,random_state=0)
from sklearn.linear_model import LinearRegression
regressor=LinearRegression()
regressor.fit(x_train,y_train)
y_pred=regressor.predict(x_test)
y_pred
plt.scatter(x_train,y_train,color="orange")
plt.plot(x_train,regressor.predict(x_train),color="red")
plt.title("Hours vs Scores(Training Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show()
plt.scatter(x_test,y_test,color="purple")
plt.plot(x_test,regressor.predict(x_test),color="yellow")
plt.title("Hours vs Scores(Training Set)")
plt.xlabel("Hours")
plt.ylabel("Scores")
plt.show() 
*/
```

## Output:
![2024-02-19](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/d03a59d9-16b9-4d90-80e8-6277ba85321a)
![2024-02-19 (2)](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/bb93cfa5-93df-4e57-aa26-650af85aa02d)
![2024-02-19 (3)](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/3b535a4c-4ab1-4a53-b34b-7d4d5310c2e2)
![2024-02-19 (4)](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/5e6eb4e4-880c-4ca2-a430-c2426a48ca90)
![2024-02-19 (5)](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/bd1c1414-59c3-4877-88bb-e25c233d731d)
![2024-02-19 (6)](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/253e3dd1-f151-459d-b195-fce46e030599)
![2024-02-19 (7)](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/307fdc16-0173-4af9-b0c6-f477e34e9fac)








## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
