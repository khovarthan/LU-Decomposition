# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program and import the required library (numpy).
2. Initialize the matrix for which the LU decomposition needs to be found.
3. Apply LU Decomposition
4. Display the results

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: khovarthan.v
RegisterNumber: 212225220052
*/
```
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Khovarthan.v
RegisterNumber: 212225220052
*/
```
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
b= np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:
(i) To find the L and U matrix
<img width="1167" height="850" alt="image" src="https://github.com/user-attachments/assets/99a3f5b7-f4bb-4f41-a4c3-2b1f656a5cfd" />
(ii) To find the LU Decomposition of a matrix
<img width="1225" height="852" alt="image" src="https://github.com/user-attachments/assets/8c48ebc8-2318-4dde-9fc0-970d1386ebf7" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

