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
<img width="1152" height="437" alt="MA EX;5 1" src="https://github.com/user-attachments/assets/11091c98-8148-4ef9-bb22-2ab673afa75b" />
(ii) To find the LU Decomposition of a matrix
<img width="1064" height="238" alt="MA EX;5 2" src="https://github.com/user-attachments/assets/908c1b71-3072-49af-bccd-ca90012219e2" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

