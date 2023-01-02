# **MLEM_Iterative_Image_Reconstruiction**

**Radon Transformation (From Wikipedia)**

In mathematics, the Radon transform is the integral transform which takes a function f defined on the plane to a function A*f defined on the (two-dimensional) space of lines in the plane, whose value at a particular line is equal to the line integral of the function over that line. 
Basically, the radon transformation representing the creation of a projection data obtained from laser scan on some object

**The Project**

In this project I am using the radon transformation in order to create a projection matrix, the sinogram, of a grayscale image object. The original image can be recovered from its sinogram by solving an optimization problem- for image x we would like to minimize f(x)  while f is the negative log-liklihood function. 
Due to the fact that f(x) is a convex function, the problem can be solved using the projected subgradient method, and by choosing a specific step size this problem becomes the classic MLEM (Maximum Likelihood Expectation Minimization) algorithm. 

The formulated algorithm can be found in the following paper:
https://web.stanford.edu/~pratx/PDF/DMLEM.pdf

In adittion, the python notebook contains some additional explanation for describing the operation I am implementing in each code block.
