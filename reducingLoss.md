# Reducing Loss

Now that we have some notion of error, we can try and optimize our model by minimising the error it produces.

This can be done by starting at some arbitrary value for the weights, calculating the derivative of loss with respect to the weights, and then moving in the negative direction of this derivative. 

The amount we move by is referred to as the *learning rate*. A small learning rate may take a while to converge on the optimal weight so we may choose to increase the learning rate. However, if the error produced by this new weight is greater than the error produced by the previous weight, the system will *diverge* from the optimal weight value.

The initial value we pick for the weight may have a large impact on the weight value that we converge on. This could occur if the function we are trying to learn is not *convex* (bowl shaped), a common occurence in machine learning.


## Efficiency

It may not be necessarily too efficient to compute the loss at each step of gradient descent. In practise, it may be sufficient to only compute the loss of a few data points.

Stochastic gradient descent: Random value chosen and the loss is computed for that value
Mini-batch stochastic gradient descent: Random sample chosen (normally 10-100 samples) and the mean loss is computed for these

