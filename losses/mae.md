# Mean Absolute Error

## MAE minimize medians

Lets say you have a distribution $Y$ and modelling it with some value $\hat{y}$

This time we are going to use a different loss function, mean absolute error (mae) 

$mae = \frac{1}{N} \sum |y_i - \hat{y}|$

Simiarly we take the derivative, interestingly the derivative of $|x|$ is 1 or -1 depending on whether x > 0 or x < 0. 

so the derivative is 

$mae_{\hat{y}} = \frac{1}{N} (\sum_{x>0} 1 + \sum_{x<0}{-1})$

Which means if we want to minimize this, then we want 50% of $y_i$ above $\hat{y}$ and 50% below.. which you might have guessed is the median 
