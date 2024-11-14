# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the necessary python packages using import statements.
2. Read the given cs file using read _csv) method and print the number of contents to be dislayed using df.head.
3. Split the dataset using train_test_split. 4.Calculate Y_pred and accuracy.
4. Print all the outputs.
5. End the program.
## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: ARAVIND G
RegisterNumber: 212223240011 
*/
```
import pandas as pd data= pd.read_csv("C:/Users/admin/Desktop/INTR MACH/spam.csv", encoding= 'Windows-1252') data.head )
data.info)
data.isnull().sum)
x=data["v1"].values y=data["v2"].values
from sklearn.model_selection import train_test_split
x_ train,x_test, y_train, y_test = train_test _splif(x,y, test_size=0.2, random_state=0)
from sklearn.feature_extraction.text import CountVectorizer
Cv=CountVectorizer()
x_train = cv.fit_transform(x_train)
x_test= cv.transform(x_test)
from sklearn.svm import SVC
svC=SVCQ
svc.fit(x_train, y_train) y pred=svc.predict(x_test)
Y pred from sklearn import metrics
accuracy = metrics.accuracy_score(y_test, y_pred)
accuracy
from sklearn.metrics import confusion_matrix, classification_report con= confusion_miatrixy_test, y_pred)
print(con)cl = classification reporty_test,y_pred)
print(cl)
## Output:
![Screenshot 2024-11-14 223951](https://github.com/user-attachments/assets/fb4eb750-3029-47c1-871b-f5efaba0e8d5)
![Screenshot 2024-11-14 224009](https://github.com/user-attachments/assets/439b5c85-8dcf-4093-8346-005e02d792e9)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
