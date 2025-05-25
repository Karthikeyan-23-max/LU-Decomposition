# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

1. **Read** a matrix $A$ from user input and convert it to a NumPy array.
2. **Perform** LU decomposition using `scipy.linalg.lu(A)`.
3. **Extract** the matrices $L$ (lower) and $U$ (upper) from the result.
4. **Print** the matrices $L$ and $U$.


## Program:
(i) To find the L and U matrix
```
'''
Program to find the L and U matrix.
Developed by: Karthikeyan C
RegisterNumber: 212224040152
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```

## Algorithm

1. **Input** matrix $A$ and vector/matrix $B$ from the user.
2. **Perform** LU factorization of $A$ using `lu_factor()`.
3. **Solve** the system $AX = B$ using `lu_solve()` with the LU result.
4. **Print** the solution vector/matrix $X$.


## Program
(ii) To find the LU Decomposition of a matrix
```
'''
Program to find the LU Decomposition of a matrix.
Developed by: Karthikeyan C
RegisterNumber: 212224040152
'''
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
piv,lu=lu_factor(A)
result=lu_solve((piv,lu),B)
print(result)
```

## Output:
![alt text](<ex-05 (1).png>)
![alt text](<ex-05 (2).png>)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

