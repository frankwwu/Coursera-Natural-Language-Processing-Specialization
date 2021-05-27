# Optional Logistic Regression: Gradient

This is an optional reading where I explain gradient descent in more detail. Remember, previously I gave you the gradient update step, but did not explicitly explain what is going on behind the scenes. 
The general form of gradient descent is defined as:

Repeat{θj:=θj−α∂∂θjJ(θ)}

For all jj. We can work out the derivative part using calculus to get:

Repeat{θj:=θj−αm∑i=1m(h(x(i),θ)−y(i))x(i)j}

A vectorized implementation is:

\theta := \theta - \frac{\alpha}{m} X^{T} (H(X , \theta ) - Y)θ:=θ− 
m
α
​	
 X 
T
 (H(X,θ)−Y)

## Partial derivative of J(θ)

First calculate derivative of sigmoid function (it will be useful while finding partial derivative of J(θ)):

h(x)′=(11+e−x)′=−(1+e−x)′(1+e−x)2=−1′−(e−x)′(1+e−x)2=0−(−x)′(e−x)(1+e−x)2=−(−1)(e−x)(1+e−x)2=e−x(1+e−x)2=(11+e−x)(e−x1+e−x)=h(x)(+1−1+e−x1+e−x)=h(x)(1+e−x1+e−x−11+e−x)=h(x)(1−h(x))

Note that we computed the partial derivative of the sigmoid function. If we were to derive  h(x^{(i)}, \theta)h(x 
(i)
 ,θ) with respect to \theta_jθ 
j
​	
 , you would get h(x^{(i)}, \theta)(1-h(x^{(i)}, \theta))x^{(i)}_jh(x 
(i)
 ,θ)(1−h(x 
(i)
 ,θ))x 
j
(i)
​	
 . Note that we used the chain rule there, because we multiply by the derivative of \theta^Tx^{(i)} θ 
T
 x 
(i)
   with respect to \theta_jθ 
j
​	
 . Now we are ready to find out resulting partial derivative:

∂∂θjJ(θ)=∂∂θj−1m∑i=1m[y(i)log(h(x(i),θ))+(1−y(i))log(1−h(x(i),θ))]=−1m∑i=1m[y(i)∂∂θjlog(h(x(i),θ))+(1−y(i))∂∂θjlog(1−h(x(i),θ))]=−1m∑i=1m⎡⎣⎢y(i)∂∂θjh(x(i),θ)h(x(i),θ)+(1−y(i))∂∂θj(1−h(x(i),θ))1−h(x(i),θ)⎤⎦⎥=−1m∑i=1m⎡⎣⎢y(i)∂∂θjh(x(i),θ)h(x(i),θ)+(1−y(i))∂∂θj(1−h(x(i),θ))1−h(x(i),θ)⎤⎦⎥=−1m∑i=1m⎡⎣⎢y(i)h(x(i),θ)(1−h(x(i),θ))∂∂θjθTx(i)h(x(i),θ)+−(1−y(i))h(x(i),θ)(1−h(x(i),θ))∂∂θjθTx(i)1−h(x(i),θ)⎤⎦⎥=−1m∑i=1m⎡⎣⎢y(i)h(x(i),θ)(1−h(x(i),θ))∂∂θjθTx(i)h(x(i),θ)−(1−y(i))h(x(i),θ)(1−h(x(i),θ))∂∂θjθTx(i)1−h(x(i),θ))⎤⎦⎥=−1m∑i=1m[y(i)(1−h(x(i),θ))x(i)j−(1−y(i))h(x(i),θ)x(i)j]=−1m∑i=1m[y(i)(1−h(x(i),θ))−(1−y(i))h(x(i),θ)]x(i)j=−1m∑i=1m[y(i)−y(i)h(x(i),θ)−h(x(i),θ)+y(i)h(x(i),θ)]x(i)j=−1m∑i=1m[y(i)−h(x(i),θ)]x(i)j=1m∑i=1m[h(x(i),θ)−y(i)]x(i)j

The vectorized version:

\nabla J(\theta) = \frac{1}{m} \cdot  X^T \cdot \left(H\left(X, \theta\right) - Y\right)∇J(θ)= 
m
1
​	
 ⋅X 
T
 ⋅(H(X,θ)−Y)

Congratulations, you now know the full derivation of logistic regression :) !