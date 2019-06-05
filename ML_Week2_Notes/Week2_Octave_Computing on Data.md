## Octave Computing on Data

-----------------------------------------
- A is matrix with 3 by 2
- B is matrix with 3 by 2 (A diff from B)
- C is matrix with 2 by 2
- V is vector with 4 by 1
------------------------------------------

Function | Interpretation
---------|---------
A * B  | matrix mutplication 
A .* B | each element in A copresspondingly multiply each element in B 
A .+ B | each element in A copresspondingly plus each element in B 
A .^ 2 | each element in A is copresspondingly squared 
A ^ 2 | equal to A * A, different from A .^ 2
1 ./ A | each element in A is copresspondingly devided by 1 
C (r*c) .sign D  | elementwise computing require D has dim 1 * c or r * c 
log (A) | elementwised logarithm
exp(A) | elementwised exponential
abs(A) | elementwised absolute value
-A = (-1*A) |elementwised negative  
A + ones(size(A)) = A + 1 |each element in A plus 1
A' | transpose A (转置)
max(A) |find seperately maximum number in row and col
max(V) |find maximum number in this vector
[val, ind] = max(V) |find maximal value and coresponding index
V < 3 |This is elementwise comparison
find (V < 3) |find element is less than 3 and output index of elements
magic([#>2]) |generate magic sqaure with each row/col/diaginals summation equal (num should be larger than 2)
[r,c] = find(A >=7) |find Value larger or equal to 7 in matrix A and output index of A and r is row indix and c is col indix repectively.
sum (V,(dim)), prod(V,(dim)) | sum or multiply each element in V
floor(V) |elementwised round down
ceil (V) |elementwised round up 
max (rand(3),rand(3)) |elementwise comparison of each matrix and output new matrix|
max (A, [], dim) |find maximal value in each sepcified dimension in matrix A
 _max(A) = max(A,[],1)_
 _max(max(A))_ |output is single value
 _max(A(:)), A(:)_ |transfer matrix to be vector
eye(#) |generate diaginal identity matrix
flipud(A) |flip matix vertically
pinv(A) |pseudo-inverse, inverse matrix (逆)
std(vector)|calculate standard deviation of this vector





