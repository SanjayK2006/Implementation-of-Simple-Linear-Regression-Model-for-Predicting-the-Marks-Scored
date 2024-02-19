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
y_test
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
mse=mean_squared_error(y_test,y_pred)
print("MSE =",mse)
mae=mean_absolute_error(y_test,y_pred)
print("MAE =",mae)
rmse=np.sqrt(mse)
print("RMSE =",rmse)
*/
```

## Output:
![Screenshot 2024-02-19 211330](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/698c1ae2-6655-4a3b-90a9-0cc13e4e1022)
![Screenshot 2024-02-19 211347](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/4be3433c-27e6-4cac-8178-bf8dbf6ae978)
![Screenshot 2024-02-19 211347](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/b1cd39b3-f900-4d90-83e2-e3d84ec5ca77)
![Screenshot 2024-02-19 211628](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/960c9151-12e6-457a-8332-d187a264d713)
![Screenshot 2024-02-19 211656](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/11b30918-513f-4e2f-ac17-cd3cd1ea015e)
![Screenshot 2024-02-19 211716](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/85ca4841-10b9-4f37-8b44-adb91c37bc67)
![Screenshot 2024-02-19 211742](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/ba252bad-8c9c-4495-b06c-639f2d9274f4)
![Screenshot 2024-02-19 211757](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/7dcbda77-91f0-40a1-8375-0634bcd6ec34)
![Screenshot 2024-02-19 211815](https://github.com/SanjayK2006/Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored/assets/144979178/77ebe46d-e84b-4a2f-9586-5520724ca88d)







## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
