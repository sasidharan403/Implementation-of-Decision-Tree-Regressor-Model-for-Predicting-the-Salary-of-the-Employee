# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required libraries.
2. Upload the csv file and read the dataset.
3. Check for any null values using the isnull() function.
4. From sklearn.tree inport DecisionTreeRegressor.
5. Import metrics and calculate the Mean squared error.
6. Apply metrics to the dataset, and predict the output.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by:A.sasi dharan 
RegisterNumber: 212221240049

import pandas as pd
data = pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data["Position"] = le.fit_transform(data["Position"])
data.head()
x = data[["Position","Level"]]
y = data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt = DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
mse = metrics.mean_squared_error(y_test,y_pred)
mse
r2 = metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:

### Data Head:
![mlex6 1](https://user-images.githubusercontent.com/94154712/173537861-bca1456d-0645-48ef-ba55-6f0c3cdec93f.png)

### Data Info:
![ml6 2](https://user-images.githubusercontent.com/94154712/173537919-c3da5139-3243-4222-bf23-d0fc52ea1e92.png)

### Data Head after applying LabelEncoder():
![ml6 3](https://user-images.githubusercontent.com/94154712/173537982-6b67e9f1-505d-48b1-b4f5-ba722f8dc6c1.png)

### MSE:
![ml6 4](https://user-images.githubusercontent.com/94154712/173538057-50104f13-c804-448d-a3ba-1a748efa0e87.png)

### r2:
![ml6 5](https://user-images.githubusercontent.com/94154712/173538196-8a496a70-a82e-40aa-9679-5aa4bf890024.png)


### Data Prediction:
![ml6 6](https://user-images.githubusercontent.com/94154712/173538245-c1caff3f-b8f2-4534-bd86-a859fd4b15f9.png)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
