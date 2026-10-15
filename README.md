# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:
##5a Algorithm
1. import os and numpy module packages and import lu from scipy.linalg.
2. Get input and convert to matrix form in the code.
3. Find the L and U matrices in code and store in variables.
4. Print the result.

##5b Algorithm
1. import os and numpy module packages and import lu_solve and lu_factor from scipy.linalg.
2. Receive inputs from user and convert it to matrices in code.
3. Solve using the inputs and find the LU Decomposition.
4. Print the result.

## Program:
(i) To find the L and U matrix
```
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
```
(ii) To find the LU Decomposition of a matrix
```
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
```

## Output:
Program(5a)
<img width="1482" height="866" alt="image" src="https://github.com/user-attachments/assets/c213854d-ae07-46c5-941d-bdf84eef6d27" />
Output(5a)
<img width="1456" height="940" alt="image" src="https://github.com/user-attachments/assets/51a1e41a-ba4b-4920-bdcc-b9ca709b5f98" />

Program(5b)
<img width="1470" height="907" alt="image" src="https://github.com/user-attachments/assets/611d729a-3809-403c-adbc-964321dea671" />
Output(5b)
<img width="1312" height="897" alt="image" src="https://github.com/user-attachments/assets/300c8804-3656-4b80-b21f-7a854e90411e" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

