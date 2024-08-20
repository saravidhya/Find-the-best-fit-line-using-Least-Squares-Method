# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Vidhiya Lakshmi S
RegisterNumber: 212223230238
import numpy as np
import matplotlib.pyplot as plt
x=eval(input())
y=eval(input())
xmean=np.mean(x)
ymean=np.mean(y)
num=0
den=0
for i in range(len(x)):
  xd=x[i]-xmean
  yd=y[i]-ymean
  a=xd*yd
  num=num+np.sum(a)
  b=xd**2
  den=den+np.sum(b)
m=(np.sum(num))/(np.sum(den))
c=ymean-m*xmean
print(m,c)
y_predicted = m*(x+b)
print(y_predicted)
plt.scatter(x,y)
plt.plot(x,y_predicted)
plt.show()
*/
```

## Output:
![image](https://github.com/user-attachments/assets/dbd404ea-ec00-4734-a615-c11730d056d7)


## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
