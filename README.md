# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
(i)
1. Importing Numpy module package and lu function from Scipy package
2. Getting the matrix input and storing it in a variable
3. Finding the L and U matrix using the lu function
4. Printing the result

## Program:
(i) To find the L and U matrix
```
/*
'''Program to find L and U matrix using LU decomposition.
Developed by: Sre Vishnu Priyar L N
RegisterNumber: 26009605
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
'''Program to solve a matrix using LU decomposition.
Developed by: Sre Vishnu Priyar L N
RegisterNumber: 26009605
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)
*/
```

## Output:
Output For 1st Program
<img width="1456" height="940" alt="image" src="https://github.com/user-attachments/assets/51a1e41a-ba4b-4920-bdcc-b9ca709b5f98" />
Output For 2nd Program
<img width="1312" height="897" alt="image" src="https://github.com/user-attachments/assets/300c8804-3656-4b80-b21f-7a854e90411e" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

