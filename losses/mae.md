# Mean Absolute Error

## MAE minimize medians

Lets say you have a distribution $Y$ and modelling it with some value $\hat{y}$

This time we are going to use a different loss function, mean absolute error (mae) 

$mae = \frac{1}{N} \sum |y_i - \hat{y}| $

Simiarly we take the derivative, interestingly the derivative of $|x|$ is 

$\left\{ 
  \begin{array}{ c l }
    1 & \quad x \gt 0 \\
    -1  & \quad x \lt 0
  \end{array}
\right.$

so the derivative is 

$mae'_{\hat{y}} = \frac{1}{N} (\sum_{x>0} 1 + \sum_{x<0}{-1})$

Which means if we want to minimize this, then we want 50% of $y_i$ above $\hat{y}$ and 50% below.. which you might have guessed is the median 
