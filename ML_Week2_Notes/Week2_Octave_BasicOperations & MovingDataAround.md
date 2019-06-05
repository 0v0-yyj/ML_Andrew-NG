#### Basic Operations
-------------------------------

Function | operation in Matlab
---------|---------------------
help func | pop up function detail and usage
eye (#) | generate diagonal identity matrix
hist(dataset, [#ofBins]) | plot histogram (default 10 bins)
rand (r,c)| randomly generate matrix with r*c dim from U(0,1)
ones (r,c); zeros(r,c) | generate all 1/0 matrix with r*c dim. _if one var x, then x*x dim
disp(a) | shows a value
sprint('string:', %0.2f, a) |%() format print, 0.2f means before 0 keep the same and keep 2 decimals for this __floating num__ print "string: a value with 2 decimals"
PS1('')| change prompt in command window
11; xor(a,b)| logical OR
&& |logical AND
~= |Not Equal

&nbsp;
&nbsp;


#### Basic Operations
-------------------------------

Function | operation in Matlab
---------|---------------------
[A B] | concatenate mateix A and B
[A; B]| attach matrix B followed by matrix A
A(:) |transpose matrix A to be column vector
A(:,2 = [a,b,c]) | replace elements in matrix
save [filename.format] [var] | save the var into filename.format
clear a or clear ('a')|clear var a in current scope, no any specification then clear all var in scope
who| show all var in current memory
whos | shows all var in current memeory with details
load(dataset)|load dataset into current scope could be txt/excel...
length(vector)| show # of elements in this vector, if matrix, then show max(length(rows),length(cols))
size(matrix)| show number of rows and cols for matirx row*col
