Assumptions
-----------------------------------------
  A is matrix with 3 by 2
	B is matrix with 3 by 2 (A diff from B)
	C is matrix with 2 by 2
	V is vector with 4 by 1
------------------------------------------

|1. A * B  |matrix mutplication|
2. A .* B |each element in A copresspondingly multiply each element in B|
3. A .+ B |each element in A copresspondingly plus each element in B|
4. A .^ 2 |each element in A is copresspondingly squared|
5. 1 ./ A |each element in A is copresspondingly devided by 1|
6. + log (A)
   + exp(A) 
   + abs(A) 
   + -A (-1*A) |each element in A execute respective function
7. A + ones(size(A)) = A + 1 |each element in A plus 1|
8. A' | transpose A (转置)|
9. max(A) |find seperately maximum number in row and col|
   + max(V) |find maximum number in this vector|
   + [val, ind] = max(V) |find maximal value and coresponding index|
10.V < 3 |This is elementwise comparison|
11. find (V < 3) |find element is less than 3 and output index of elements|
12. magic([#>2]) |generate magic sqaure with each row/col/diaginals summation are equal|
13. [r,c] = find(A >=7) %find Value larger or equal to 7 in matrix A and output index of A
    and r is row indix and c is col indix repectively.
14. sum (V,(dim)), prod(V,(dim)) % sum or multiply each element in V
15. + floor(V) %round down
    + ceil (V) %round up
16. max (rand(3),rand(3)) |elementwise comparison of each matrix and output new matrix|
17. max (A, [], dim) |find maximal value in each sepcified dimension in matrix A|
	+ max(A) = max(A,[],1)
	+ max(max(A)) is single value
	+ max(A(:)), A(:) %transfer matrix to be vector
18. eye(#) |generate diaginal identity matrix|
19. flipud(A) |flip matix vertically|
20. pinv(A) |pseudo-inverse, inverse matrix (逆)|




