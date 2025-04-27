# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import required libraries numpy and scipy.linalg
2. Input the matrix/matrices using eval(input()).
3. Perform LU decomposition using lu() or solve equations using lu_factor() and lu_solve()
4. Print the results L and U matrices or solution X matrix

## Program:
(i) To find the L and U matrix
```python
/*
Program to find the L and U matrix.
Developed by: CHARUKESH S 
RegisterNumber: 212224230044
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
/*
Program to find the LU Decomposition of a matrix.
Developed by: CHARUKESH S
RegisterNumber: 212224230044 
*/
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
# (i)to find L and U matrix using LU decomposition
![image](https://github.com/user-attachments/assets/5870c6d0-0315-4289-855b-0116668fa431)
# (ii)to solve a matrix using LU decomposition.
![image](https://github.com/user-attachments/assets/1a1f5949-f458-40d1-87cc-a6597711cc03)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

