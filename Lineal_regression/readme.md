# The lineal regresion
This is one of the simplest methods on machine learning, and it is one of the most important. To look it throught the regression, we need to see, how is it
$$y=\beta_0+\beta_1x_i$$
The linear regression follows a simple lineal function. With this aim, we can have several of its properties, such as the slop and intercept.

Now, we are agree, that $x_i$, is an element from a big vector denominated as $X$, thus, it can be simplified this expression as 

$$Y=\beta X$$

$Y$ is also a vector, and one of the main problems that we can get stuck, how can you determine the values of $\beta$ if you only know $X$,$Y$
For taht reason we need to get into optimization, here I can let you a repository to optimizers, and these have a bigger explanation. Although, we need a simple approach.

When you track a line into data, it will be seen that several dots will not fit perfectly into the line, so they will have certain distance. But, as the line is a certain predictor, determined by $\hat{y}$, and the dots are represented as $y$, my main interest is to find out how the line predicts. So it can be defined an expression that measures the distance between the dots and the values.
$$Y-\hat{Y}$$
![lineal3](https://github.com/user-attachments/assets/cf012f0c-d06c-488c-bcb1-e949b67a24cb)
So as in the image, it can be visible how the data are spread into the 2 dimensional space, and the lineal regression tries to fit on the data, however, this will not be always posible, So with the difference that it has been developed, we can see how "well" our model predicted. This is called an error.

The error is a measure that express how well a model describe certain data. There are a lot of type of errores according to the problem, nevertheless, the most common is Mean Square Error. 

$$MSE=\frac{1}{N}\sum^N_{i=0}(Y_i-\hat{Y}_i)^2$$

The reason that our difference is squared, is due to we are not interest in the direction of the distance, because the difference can express if the dot is up or down of the line, but is not matter to know. For that reason we need to look through positive values.
At this way, you can measure the error from the dots and the model, also, you can know if you put values on X, what can be the output, but, how can you make a model that fits on a certain data?

Take in mind, before to take in hand the data with model, it is fundamental to know that the data follows a normal distribution, for this we actually need to make tests like Shapiro-Wilk, to know if our data follows a normal distribution. Therefore, as we need to fit a model into the data, the parameters that we don't know, are  $\beta$, so the great question is how can you find out the best parameters for our model?, for that reason we need optimizers.

The most well known optimizers are diferentiable, so it an be approach this by

$$MSE=\frac{1}{N}\sum^N_{i=0}(y_i-\beta_0-\beta_1x_i)^2$$
