# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. 
2. 
3. 
4. 

## Program:
Program to solve a matrix using Gaussian elimination without partial pivoting.

Developed by: DILLIARASU M

RegisterNumber: 212223230049

```import numpy as np
n=int(input())
matrix=np.zeros((n,n+1))
x=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        matrix[i][j]=int(input())
for i in range(n):
    for j in range(i+1,n):
        ratio=matrix[j][i]/matrix[i][i]
        for k in range(n+1):
            matrix[j][k]=matrix[j][k]-ratio*matrix[i][k]
#Back substitution
x[n-1]=matrix[n-1][n]/matrix[n-1][n-1]
for i in range(n-2,-1,-1):
    x[i]=matrix[i][n]
    for j in range(i+1,n):
        x[i]=x[i]-matrix[i][j]*x[j]
    x[i]=x[i]/matrix[i][i]
for i in range(n):
    print("X%d = %0.2f" %(i,x[i]),end=" ")
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: 
RegisterNumber: 
*/
```

## Output:
![Screenshot 2024-04-04 201641](https://github.com/Dilliarasu0105/Gaussian/assets/144979593/99bffb27-0159-4a84-adb7-57663ed8eec3)
![Screenshot 2024-04-04 201702](https://github.com/Dilliarasu0105/Gaussian/assets/144979593/7dc9aa73-cf12-466d-bf47-3a296d6c69d9)




## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

