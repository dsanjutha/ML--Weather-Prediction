# Implementation of Random Forest Algorithm for Weather Prediction
## AIM:
To write a program to predict daily temperature , PM2.5 pollution level and Energy based on environmental sensor data using Random Forest Algorithm.

## Problem Statement and Dataset



## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
```

1.Start the program.
2.Read two input numbers from the user:
  *.First number → A
  *.Second number → B
3.Perform addition operation:
  *.Add A and B
  *.Store the sum in a variable called Result
4.Display the value of Result on the screen.
5.Stop the program.

```

## Program:
```python
/*
Program to implement the Random Forest Algorithm to predict daily temperature , PM2.5 pollution level and Energy based on environmental sensor data.
Developed by: sanjutha D
RegisterNumber: 212225240136
import numpy as np
from sklearn.ensemble import RandomForestRegressor
from sklearn.model_selection import train_test_split

X = np.array([
    [70, 5, 1012],
    [65, 7, 1010],
    [80, 4, 1008],
    [75, 6, 1011],
    [60, 8, 1013],
    [85, 3, 1007],
    [90, 2, 1006],
    [55, 9, 1014]
])

Y = np.array([
    [30, 80, 200],
    [28, 70, 180],
    [32, 90, 220],
    [29, 75, 190],
    [27, 65, 170],
    [33, 95, 230],
    [34, 100, 240],
    [26, 60, 160]
])

X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=0.2, random_state=0)
model = RandomForestRegressor(n_estimators=100, random_state=0)
model.fit(X_train, Y_train)
Y_pred = model.predict(X_test)
print("Predicted Values (Temperature, PM2.5, Energy):", Y_pred)
sample = np.array([[72, 5, 1011]])
prediction = model.predict(sample)
print("Prediction for new data (Temp, PM2.5, Energy):", prediction[0])


 
*/
```

## Output:
<img width="737" height="72" alt="image" src="https://github.com/user-attachments/assets/9f794f97-4ce9-4c77-9282-f05c197f3b29" />


## Result:
Thus the program to implement the  Implementation of Random Forest Algorithm for Weather Prediction
