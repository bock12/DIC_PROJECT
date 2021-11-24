import numpy as np

import numpy as np

a = np.array([[-1,2,3]])
b = np.array([[0,2,1]])
np.dot(a,b)
```
[![Image from Gyazo](https://t.gyazo.com/teams/diveintocode/e9e3c6e91b7d4abd99001aa0848e4059.png)](https://diveintocode.gyazo.com/e9e3c6e91b7d4abd99001aa0848e4059)

Thank you for the question. The problem you are trying to solve is a matrix multiplication problem.  Two matrices can only be multiplied when the number of columns of the first matrix is equal to the number of rows of the second matrix.

a.ndim


b.ndim

When yoy check the shape of the two variable a and b, you will notice that both have the same dimension.<br> So to solve the problem, you change the shape of the second matrix which appen to be b as shown below.

b = b.reshape(3, 1)
b

Now the the we have changed the shape of the variable, we will now execute the code to see the outcome.

a = np.array([[-1,2,3]])
b = np.array([[0,2,1]]).reshape(3,1)
np.dot(a,b)
