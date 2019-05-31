## Octave Control Statements

------------------------------------
Learning Control Statements  
* for
* while
* if
------------------------------------

#### For Loop
```Octave
for i = 1:10,
	v(i) = 2^i; %semicolon assist to not print out
end
#break uses to halt loop;continou uses to skip this run 
```
> v                                         
> 2 4 8 16 32 64 128 256 512 1028 2056 
> :point_right:automatically identify and update vector/matrix without specifying before 
 
#### While Loop
```Octave
i = 1;
while i <= 5,
	v(i) = 100;
	i = i+1;
end;
#break and contious could be used as well
```
> v                                                  
> 100 100 100 100 100 64 128 256 512 1028 2056 

#### while + if + break Loop
```Octave
i=1,
while true, #permenant loop
	v(i) = 999;
	i = i+1
	if i == 6,
		break
	end;
end;
```

> v                                                                                                                              
> 999 999 999 999 999 128 256 512 1028 2056

#### if-else
```Octave
v(1) = 2;
if v(1) == 1,
	disp('The value is one');
else if v(1) == 2,
	disp('The value is two');
else 
	disp("The value is not one or two')
end;
```
> The value is two

#### How to define and use functions
:point_right:__Notes__:
1. "q" and "exit" would help you qiut Octave
2. Define function by creating functionName.m in Octave new funtion, open it using WordPad rather than NotePad messing up the spacing.
##### In wordPad
> function y = squaredThisNumber(x)
>
> y = x^2

* return single value y and one argument x by squared function.

##### In wordPad
> function [y1,y2] = squareAndCuberThisNumber(x)

> y1 = x^2
> y2 = x^3

* return 2 values: y1 and y2

3. if you wanna use this fucntion:
* you have to(pwd) cd to path where save this function wordPad
* :point_right: OR using addpath

``` Octave
addpath('C:\Users\Desktop)
cd "C:\"
SquareThisNumber(5)
[a,b] = squareAndCubeThisNUmber(5)
```
#### Sophisticated example of function

#### In WordPad
> function J = costFunctionJ(X, y, theta)                           
> %X is the "design matrix" containing our trainning example                             
> %y is the class labels  
>                                                                      
> m = size(X,1); %number of training examples                                                        
> prediction = X*theta % predictions of hypothesis on all m                                                                
> examples                                                                                                                           
> sqrErrors = (predictions-y).^2; %square errors                                                                          
>                                                   
> J = 1/(2*m)*sum(sqrErrors);                                         

``` Octave
X = [1,1;1,2;1,3];
y = [1;2;3];
theta1 = [0;1] :point_right:_perfectly match y value,CostFunctionJ = 0
theta2 = [0;0] :point_right:_maximal error parameters, CostFunctionJ = 2.333

(1^2+2^2+3^3)/(2*3) :point_right: equal to theta2 results
```









```

