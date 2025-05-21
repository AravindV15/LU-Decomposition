# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import required libraries numpy and scipy.linalg.

2. Input the matrix/matrices using eval(input()).

3. Perform LU decomposition using lu() or solve equations using lu_factor() and lu_solve().

4. Print the results L and U matrices or solution X matrix.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Aravind G
RegisterNumber: 212224240014
*/
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Aravind G
RegisterNumber: 212224240014 
*/
import numpy as np
from scipy.linalg import lu_factor, lu_solve
a = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(a)
x = lu_solve((lu, piv), b)
print(x)
```

## Output:

(i) L and U matrix
![image](https://github.com/user-attachments/assets/d43ade59-9d3d-4b93-adf7-13d4f327c0c6)

(ii) LU decomposition of a matrix
![image](https://github.com/user-attachments/assets/8a0057e4-684f-4226-a5f4-2d40b04108fb)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
