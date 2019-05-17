# Partial Differentiation

This is just a quick note to myself about how partial differentiation works.

Say you have a function

f(x,y,z) = x^2 - 1/y + 2zxy

Partial differentiation tells you how the output of the function changes if you only change one variable.

To do this you just take the normal derivative with respect to whatever variable you are looking at and hold the other variables constant (by just treating them as constants as you would normall).

For example, differentiating f(x,y,z) with respect to x gives:

2x - 1/y + 2zy


When computing the gradient of this function in all directions, you end up with a vector equal in dimensions to the number of parameters to the input function. This tells you how much the function changes as you take a step in each direction.

For example the gradient of f(x,y,z) is:

(2x - 1/y + 2zy,
 2x + y^-2 + 2zx,
 2x - 1/y + 2xy)

Note that the vector is listed as (dx, dy, dz)
