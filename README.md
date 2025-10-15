# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Take matrix input from the user and convert it to a NumPy array.
2.Apply LU decomposition using scipy.linalg.lu() to get P, L, and U.
3.Extract the L (lower) and U (upper) triangular matrices.
4.Print the L and U matrices 

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: VD Natchathira
RegisterNumber: 212224230178
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: VD Natchathira
RegisterNumber: 212224230178
*/
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)

```

## Output:
<img width="802" height="432" alt="Screenshot 2025-10-15 092857" src="https://github.com/user-attachments/assets/19bc50e5-1572-4801-827d-fb480f4bfe7d" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

