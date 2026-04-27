# Implementation-of-Logistic-Regression-Using-Gradient-Descent

## AIM:
To write a program to implement the the Logistic Regression Using Gradient Descent.

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
Program to implement the the Logistic Regression Using Gradient Descent.
Developed by: lavanya D
RegisterNumber:  212225040195
*/
import numpy as np

X = np.array([1, 2, 3, 4, 5])
Y = np.array([0, 0, 0, 1, 1])

w = 0
b = 0

learning_rate = 0.1
iterations = 1000

def sigmoid(z):
    return 1 / (1 + np.exp(-z))

for i in range(iterations):
    z = w * X + b
    Y_pred = sigmoid(z)
    
    dw = np.mean((Y_pred - Y) * X)
    db = np.mean(Y_pred - Y)
    
    w = w - learning_rate * dw
    b = b - learning_rate * db

print("Weight (w):", w)
print("Bias (b):", b)

predictions = sigmoid(w * X + b)
print("Predicted Probabilities:", predictions)
print("Predicted Classes:", [1 if i > 0.5 else 0 for i in predictions])
```

## Output:
<img width="836" height="84" alt="image" src="https://github.com/user-attachments/assets/6fe93507-eacf-4766-b033-0c6c0b0b1f9a" />


## Result:
Thus the program to implement the the Logistic Regression Using Gradient Descent is written and verified using python programming.

