# Mean Squared Error

## MSE minimizes means

Lets say you have some distribution $Y$ and we are modelling it with a single prediction $\hat{y}$

The loss function is then $mse = \frac{1}{N} \sum (y_i - \hat{y})^2$

Expanding to $mse = \frac{1}{N} \sum y_i^2 - 2y_i\hat{y} + \hat{y}^2$

If we want to minimize it, we just differentiate by $\hat{y}$ and find it's turning point (where it equals 0) 

$mse'_{\hat{y}} = \frac{1}{N} \sum 2\hat{y} - 2y_i = \frac{2}{N} \sum \hat{y} - \frac{2}{N} \sum y_i = 0$

Note that $\sum \hat{y} = N\hat{y}$ giving us 

$2\hat{y} - \frac{2}{N}\sum y_i = 0$

With a little rearrangement 

$\hat{y} = \frac{1}{N} \sum y_i $
