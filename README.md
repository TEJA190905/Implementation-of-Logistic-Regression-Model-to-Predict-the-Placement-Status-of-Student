# Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student

## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: M THEJESWARAN
RegisterNumber: 212223240168
*/

import pandas as pd
data = pd.read_csv("/content/Placement_Data.csv")
data.head()
data1=data.copy()
data1=data1.drop(["sl_no","salary"],axis=1)
data1.head()
data1.isnull().sum()
data1.duplicated().sum()
x=data1.iloc[:,:-1]
x
y=data1["status"]
y
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.metrics import accuracy_score
accuracy = accuracy_score(y_test,y_pred)
accuracy
from sklearn.metrics import confusion_matrix
confusion = (y_test,y_pred)
confusion
from sklearn.metrics import classification_report
classification_report1 = classification_report(y_test,y_pred)
print(classification_report1)
lr.predict([[1,80,1,90,1,1,90,1,0,85,1,85]])
```

## Output:
![Screenshot (83)](https://github.com/user-attachments/assets/48db4190-9fe7-408f-9bb8-1da36dff172d)

![Screenshot (84)](https://github.com/user-attachments/assets/623bd7b0-11e4-4e88-8e2a-718ada05aa5c)

![Screenshot (85)](https://github.com/user-attachments/assets/684e0067-1373-4fb7-a0b9-daceec01e978)

![Screenshot (86)](https://github.com/user-attachments/assets/d8930314-ea17-4eb3-8ac5-f1ff89110cff)

![Screenshot (87)](https://github.com/user-attachments/assets/60ccd110-0c63-42dd-9d0e-e85cf9fb0835)

![Screenshot (88)](https://github.com/user-attachments/assets/b30f491a-2e6c-420b-8964-851bc52e5e91)

![Screenshot (89)](https://github.com/user-attachments/assets/3254ecdc-fd7d-46c7-aae4-b32f2751c2a7)

![Screenshot (90)](https://github.com/user-attachments/assets/2a610cf8-c89f-4d92-a068-6bd8e7197b2a)

![Screenshot (91)](https://github.com/user-attachments/assets/a4e2004e-3ef9-48db-afa9-b369f3f34b9a)

![Screenshot (92)](https://github.com/user-attachments/assets/966a7a5a-860e-4b4f-acde-71193556ad12)

![Screenshot (92)](https://github.com/user-attachments/assets/841f1731-5aa2-4f9e-be75-b0048ec3b65f)

## Result:
Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
