## Octave Vectorization

### Review

#### 1. Hypothesis Equation
:point_right:__h_theta(x) = sum(j=1:n+1)[theta_j * x_j] = theta.transpose() * x__


<p align="center">
  <img width = "166" height = "63"  src="https://github.com/yjiang14/ML_Andrew-NG/blob/master/ML_Week2_Notes/ImageFolder/Hypothesis_Eqaution.PNG">
</p>

#### 2. Gradient Descent
:point_right: __theta_j = theta_j - alpha * 1/m * sum(i=1:m)[(h_theta(x_i)- y_i) * x_j_i] for all j__

*  __theta_j = theta_j - alpha * derive(CostFunction)__


<p align="right">
	<img src="https://github.com/yjiang14/ML_Andrew-NG/blob/master/ML_Week2_Notes/ImageFolder/Gradient_Descent.PNG">
</p>

### Notes:
1. Octave/Matlab has beginning index of 1 rather than 0 (Java, Python, C, C++)
2. The vectorization is more preferred than Unvectorization implementation (simpler and efficiently)
* Unvectorization

```Octave
theta = [theta1, theta2,..];
x = [x11,x12...;x21 x22;...];
prediction = 0.0;
for j = 1:n+1,
	prediction = prediction + theta(j) * x(j)
end;
```

* Vectorization

```Octave
theta = [theta1, theta2, theta3,...];
x = [x11 x12 x13...;x21 x22 x23...;x31 x32 x33..;....];
prediction = theta' * x;
```

#### 3, Vectorization with Gradient Descent Notes

<p align = "center">
	<img src="https://github.com/yjiang14/ML_Andrew-NG/blob/master/ML_Week2_Notes/ImageFolder/Vectorization_GradientDescent_Notes.PNG">
</p>
