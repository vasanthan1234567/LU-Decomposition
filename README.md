# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
I.L AND U MATRIX

1. Start the program

2.Import the necessary libraries(numpy,scipy.linalg)

3.Define the matrix using numpy

4.Use lu(),lu_solve(),lu_factor() to get the solutions

5.End the program

II.LU DECOMPOSITION

1.Get input:

2.Read the input for the matrix AMatrix from the user.
3.Read the input for the matrix BMatrix from the user.
4.Perform LU decomposition:

5.Use the lu_factor function from the scipy.linalg library to perform LU decomposition on AMatrix.
6.Store the result in XMatrix.
7.Solve the system of equations:

8.Use the lu_solve function from the scipy.linalg library to solve the system of equations using the LU decomposition.
9.Store the result in Solution.
10.Print the solution:

11.Print the Solution matrix to the console.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: VASANTHAN N
RegisterNumber: 24900250
*/
import numpy as np
from scipy.linalg import lu
InputMatrix=np.array(eval(input()),dtype='i')
piv,Lmatrix,Umatrix=lu(InputMatrix)
print(Lmatrix)
print(Umatrix)



```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: VASANTHAN N
RegisterNumber: 24900250
*/

import numpy as np
from scipy.linalg import lu_factor,lu_solve
AMatrix=np.array(eval(input()),dtype='i')
BMatrix=np.array(eval(input()),dtype='i')
XMatrix=lu_factor(AMatrix)
Solution=lu_solve(XMatrix,BMatrix)
print(Solution)

```

## Output:

i.![OUTPUT](<Screenshot 2025-01-05 154501.png>)
ii.![OUTPUT](<Screenshot 2025-01-05 173851.png>)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

