# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```

## REGISTER NUMBER : 212224100022
## COMPLETED BY : Janani Gowrisankar



import numpy as np
X= np.array(eval(input()))
Y= np.array(eval(input()))
X_mean=np.mean(X)
Y_mean=np.mean(Y)
num=0
denom=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denom=(X[i]-X_mean)**2
  m=num/denom
  c=Y_mean-m*X_mean
  print(m,c)
  Y_pred=m*X+c
  print(Y_pred)

  import matplotlib.pyplot as plt
  plt.scatter(X,Y,color='RED')
  plt.plot(X,Y_pred,color='blue')
  plt.show()

```
## Output

<img width="1021" height="827" alt="image" src="https://github.com/user-attachments/assets/5de2f546-2fd3-48f1-ab60-2eccba19e016" />

<img width="1126" height="842" alt="image" src="https://github.com/user-attachments/assets/70a84c4d-6afe-458a-a79f-68113e116ca2" />

<img width="1026" height="757" alt="image" src="https://github.com/user-attachments/assets/09368977-5409-4dc2-a7a9-698aad4f0180" />

<img width="971" height="765" alt="image" src="https://github.com/user-attachments/assets/743c98c5-5f6a-4503-88b5-6c80a3c579d1" />

<img width="1110" height="796" alt="image" src="https://github.com/user-attachments/assets/6ffa1fb3-ef89-415e-8d6e-c67381f3b808" />

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
