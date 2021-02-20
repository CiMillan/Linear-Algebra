# Linear-Algebra

When coding or solving data analysis problems, one problem that can  occur is if your code encounters a special matrix that isn't invertible,  or has an infinite number of eigenvectors, or similar. On other  occasions, for example where you are reducing dimensionality, that might  even be desirable!  So here you will find a code fragment that traps  for different types of special matrices before calling the python  inversion routine, and classifies the type of special case encountered.  

# Instructions

This function tests if a 4×4 matrix is singular, i.e. to determine if an inverse exists, before calculating it.

We use the method of converting a matrix to echelon form, and testing if this fails by leaving zeros that can’t be removed on the leading diagonal.

# Matrices in Python

In the numpy package in Python, matrices are indexed using zero for the top-most column and left-most row. I.e., the matrix structure looks like this:

A[0, 0]  A[0, 1]  A[0, 2]  A[0, 3]<br />
A[1, 0]  A[1, 1]  A[1, 2]  A[1, 3]<br />
A[2, 0]  A[2, 1]  A[2, 2]  A[2, 3]<br />
A[3, 0]  A[3, 1]  A[3, 2]  A[3, 3]

You can access the value of each element individually using,

A[n, m]

which will give the n'th row and m'th column (starting with zero). You can also access a whole row at a time using,

A[n]

Which you will see will be useful when calculating linear combinations of rows.
