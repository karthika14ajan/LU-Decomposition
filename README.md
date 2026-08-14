# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: KARTHIKA AJAN 
RegisterNumber: 212225100021
*/
import os
os.environ['OPENBLAS_NUM_THREADS']='1'
import numpy as np 
from scipy.linalg import lu
matrix=np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)
```

(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: KARTHIKA AJAN
RegisterNumber: 212225100021
*/
import os
os.environ['OPENBLAS_NUM_THREADS']='1'
import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(matrix)
result=lu_solve((piv,lu),constant)
print(result)
```


## Output:
<img width="1237" height="640" alt="Screenshot 2026-08-14 235417" src="https://github.com/user-attachments/assets/8467fe3c-bffe-45cf-a307-8c17531dbe6b" />
<img width="1237" height="577" alt="Screenshot 2026-08-14 235440" src="https://github.com/user-attachments/assets/2bd471a9-d258-495d-b171-c4646b8f02de" />

<img width="1247" height="848" alt="Screenshot 2026-08-14 235900" src="https://github.com/user-attachments/assets/f00245cd-3c1f-4bba-be65-b0ca8b9b8789" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

