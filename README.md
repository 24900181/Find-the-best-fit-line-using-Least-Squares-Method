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
Developed by: NETHRA.K
RegisterNumber:  212224230184
*/

 import numpy as np
 import matplotlib.pyplot as plt
 x=np.array(eval(input()))
 y=np.array(eval(input()))
 x_mean=np.mean(x)
 y_mean=np.mean(y)
 num=0
 denom=0
 for i in range(len(x)):
     num+=(x[i]-x_mean)*(y[i]-y_mean)
     denom+=(x[i]-x_mean)**2
     m=num/denom
     b=y_mean-m*x_mean
     print(m,b)
     y_predicted=m*x+b
     print(y_predicted)
     plt.scatter(x,y)
     plt.plot(x,y_predicted,color='red')
     plt.show()


```

## Output:

<img width="821" height="645" alt="Screenshot 2026-02-02 100757" src="https://github.com/user-attachments/assets/4e3cc527-9e67-40a5-8739-c9a10aab07a1" />

<img width="646" height="493" alt="Screenshot 2026-02-02 100823" src="https://github.com/user-attachments/assets/286db160-d336-4bae-be86-536317b02dab" />

<img width="698" height="488" alt="Screenshot 2026-02-02 100854" src="https://github.com/user-attachments/assets/c22854be-599f-45c1-b3f5-abaa0cef7850" />

<img width="637" height="484" alt="Screenshot 2026-02-02 100908" src="https://github.com/user-attachments/assets/a6498c60-eec5-416d-b92a-bc47b8cd63b4" />

<img width="644" height="502" alt="Screenshot 2026-02-02 100921" src="https://github.com/user-attachments/assets/32eb9d82-0e87-49e7-a827-54f1335b0827" />

<img width="682" height="504" alt="Screenshot 2026-02-02 100938" src="https://github.com/user-attachments/assets/e4c8e4cd-d864-444b-ab87-460f5e6073e4" />

<img width="598" height="496" alt="Screenshot 2026-02-02 100955" src="https://github.com/user-attachments/assets/66974a13-2038-4934-b8ed-434960ae18c4" />

<img width="647" height="494" alt="Screenshot 2026-02-02 101013" src="https://github.com/user-attachments/assets/1fe02449-569f-444c-af7b-837aa38de1d2" />

<img width="608" height="523" alt="Screenshot 2026-02-02 101026" src="https://github.com/user-attachments/assets/1c68f179-921a-4482-8957-bda35f5af9a3" />

## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
