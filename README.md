# Tasks

## overview

This is a prediction model made with the seattle weather file 

## Python queries
````
import pandas as pd
````
````
dataset = pd.read_csv("seattle-weather.csv")
print(dataset)
````
````
dataset.head()
````
````
X = dataset.iloc[:,:-1].values
print(X)
````
````
y = dataset.iloc[ :, -1].values
print(y)
````
````
from sklearn.model_selection import train_test_split
X_train,X_test,y_train,y_test = train_test_split(X,y,test_size=0.2,random_state=42)
````
````
print(X_train)
````
````
print(X_test)
````
````
print(y_train)
````
````
print(y_test)
````




````
