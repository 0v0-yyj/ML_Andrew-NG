## Octave Vectorization

### Review
:point_right:__h_theta(x) = sum(j=1:n+1)[theta_j * x_j] = theta.transpose() * x__
![Hypothesis Equation](http://github.com/yjiang14/ML_Andrew-NG/blob/master/ML_Week2_Notes/ImageFolder/Hypothesis_Equation.PNG)
:point_right:__theta_j = theta_j - alpha * 1/m * sum(i=1:m)[(h_theta(x_i)- y_i) * x_j_i] for all j__
* __theta_j = theta_j - alpha * derive(CostFunction)__
![Gradient_Descent](http://github.com/yjiang14/ML_Andrew-NG/blob/master/ML-Week2_Notes/ImageFolder/Gradient_Descent.PNG)
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

