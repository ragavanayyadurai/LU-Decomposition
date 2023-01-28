# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:
## Step1:
1.import numpy
## Step2:
2.From scipy.linalg import lu ,lu_factor,lu_solve respectively
## Step3:
3.Get the input of matrix values from user using eval
## Step4: 
4.Using P,L,U=lu(A) we can find L and U matrix. Using res=lu_factor(A),solution=lu_solve(res,B) we can find LU Decomposition of a matrix. 

## Program:
(i) To find the L and U matrix

```python
#Program to find L and U matrix using LU decomposition.
#Developed by: RAGAVENDRAN A
#RegisterNumber: 22008885
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix

```python
#Program to solve a matrix using LU decomposition.
#Developed by: RAGAVENDRAN A
#RegisterNumber: 22008885
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv = lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)
```

## Output:
![lu decomposition](/output3.png)
![lu decomposition](/output4.png)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

