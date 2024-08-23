# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

step1:start

step2: Get the independent variable X and dependent variable Y.

step3: Calculate the mean of the X -values and the mean of the Y -values.

step4: Find the slope m of the line of best fit using the formula. 

<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">

step5: Compute the y -intercept of the line by using the formula:

<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">

step6: Use the slope m and the y -intercept to form the equation of the line.

step7: Obtain the straight line equation Y=mX+b and plot the scatterplot.

step8: end

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: vellachi tilak  
RegisterNumber:  212223240172

/*

import numpy as np
import matplotlib.pyplot as plt
# Preprocessing Input data
X = np.array(eval(input()))
Y = np.array(eval(input()))
#Mean
X_mean =np.mean(X)
Y_mean =np.mean(Y)
num=0 #for slope
denom=0#for slope
#to find sum of (xi-x') & (yi-y') & (xi-x')^2
for i in range(len(X)):
    num+=(X[i] -X_mean)*(Y[i]-Y_mean)
    denom+= (X[i]-X_mean)**2
#calculate slope    
m=num/denom
#calculate intercept
b=Y_mean-m*X_mean
print(m,b)
#line equation
y_predicted=m*X+b
print(y_predicted)
#to plot graph
plt.scatter(X,Y)
plt.plot(X,y_predicted,color='red')
plt.show()



```

## Output:
## slop and y-intercept

![image](https://github.com/user-attachments/assets/eeb03e20-9ea1-4fee-ad92-2c08812e970e)

## y-predicted

## GRAPH
![image](https://github.com/user-attachments/assets/749673af-8881-4a4f-83e2-ac3eafcb6125)




## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
