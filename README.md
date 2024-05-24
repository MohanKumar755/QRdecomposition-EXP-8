# Algorithm for QR Decomposition
## Aim:
To implement QR decomposition algorithm using the Gram-Schmidt method.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Intialize the matrix Q and u
2.	The vector u and e is given by

    ![eqn1](./ex4.jpg)

    ![eqn2](./ex6.jpg)

    ![eqn3](./ex3.jpg)

3.	Obtain the Q matrix   
    ![eqn4](./ex1.jpg)
4.	Construct the upper triangular matrix R
    ![eqn5](./ex2.jpg)



## Program:
```
def QR Decomposition(A):
    n, m A. shape # get the shape of A 
    Q= np.empty((n, n)) # initialize matrix Q 
    u-np.empty((n, n)) # initialize matrix u
    u[:, 0] = A[:, 0]
    Q[:, ]u[:, 8] / np.linalg.norm(u[:, 0])
QRdecomposition/README.md at main D
    for i in range(1, n): 
        u[:, i] = A[:, 1]
    for j in range(i):
        u[:, 1] -=(A[:, 1] @ Q[:, j]) Q[:, j] # get each u vector
    Q[:, i]=u[:, i] / np.linalg.norm(u[:, i]) # compute each e vetor
    R=np.zeros((n, m))
    for i in range(n):
        for j in range(i, m):
            R[i, j]= A[:, j] @ Q[:, i]
            print(Q)
            print(R)
a =np.array(eval(input()))
QR_Decomposition(a)

```
## Output
![Screenshot 2024-05-24 195947](https://github.com/MohanKumar755/QRdecomposition-EXP-8/assets/146155007/e7b8c21e-e2ec-4740-9c55-922c29ae0dab)

[[1,1,0], [1,0,1], [0,1,1]]

[[ 0.70710678 0.40824829 -0.57735027]

[ 0.70710678 -0.40824829 0.57735027]

[0             0.81649658 0.57735027]]

[[1.41421356 0.70710678 0.70710678]
[0
.           1.22474487 0.40824829]

[0.      0        1.15470054]]
## Result
Thus the QR decomposition algorithm using the Gram-Schmidt process is written and verified the result.
