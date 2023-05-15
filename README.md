# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import dataset and print dataset info
2. check for null value
3. Map numerical values for salary feature
4. Assign x and y values
5. Split the dataset into train and test sets
6. Import decisiontree classifier and fit it in the dataset
7. Find accuracy and predict values

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by:S.SRIMATHI
RegisterNumber:212220040160 

import pandas as pd

data=pd.read_csv('/content/Employee.csv')

data.head()

data.info()

data.isnull().sum()

data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder

le=LabelEncoder()

data["salary"]=le.fit_transform(data["salary"])

data.head()

x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]

x.head()

y=data["left"]

from sklearn.model_selection import train_test_split

x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)

from sklearn.tree import DecisionTreeClassifier

dt=DecisionTreeClassifier(criterion="entropy")

dt.fit(x_train,y_train)

y_pred=dt.predict(x_test)

from sklearn import metrics

accuracy=metrics.accuracy_score(y_test,y_pred)

accuracy

dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:

## DATA.HEAD():
![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/114581999/621cc909-d881-468e-b3c3-82d442827d83)
## DATA.INFO():
![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/114581999/cdf78355-883c-4bb6-bb6b-4e9970c416d9)
## ISNULL() AND SUM():
![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/114581999/3dfc8001-34e9-4aca-9910-a6132db3a20a)
## DATA VALUE COUNTS:
![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/114581999/12713ebc-2ee7-481b-8fae-f5e0abc87dc8)
## DATA.HEAD() FOR SALARY:
![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/114581999/b3e819d8-abc1-4d5c-8cfb-fe9f7267b063)
## X.HEAD()
![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/114581999/7c6d2161-9875-41d2-97bb-e3e41ece849b)
## ACCURACY VALUE:
![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/114581999/de7e8e46-efea-4226-a3a8-ffe240a69cff)
## DATA PREDICTION:
![image](https://github.com/srimathi-25/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/114581999/f4b8afc1-36f2-452a-8f86-ffbb99027c00)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
