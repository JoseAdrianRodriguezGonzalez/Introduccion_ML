# The lineal regresion
This is one of the simplest methods on machine learning, and it is one of the most important. To look it throught the regression, we need to see, how is it
$$y=\beta_0+\beta_1x_i$$
The linear regression follows a simple lineal function. With this aim, we can have several of its properties, such as the slop and intercept.

Now, we are agree, that $x_i$, is an element from a big vector denominated as *$X$*, thus, it can be simplified this expression as 

$$Y=\betaX$$
$Y$ is also a vector, and one of the main problems that we can get stuck, how can you determine the values of $\beta$ if you only know $X$,$Y$
For taht reason we need to get into optimization, here I can let you a repository to optimizers, and these have a bigger explanation. Although, we need a simple approach.

When you track a line into data, it will be seen that several dots will not fit perfectly into the line, so they will have certain distance. But, as the line is a certain predictor, determined by $\hat{y}$, and the dots are represented as $y$, my main interest is to find out how the line predicts. So it can be defined an expression that measures the distance between the dos and the values.
$$Y-\hat{Y}$$
