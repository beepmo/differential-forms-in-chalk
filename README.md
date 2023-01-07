# differential-forms-in-chalk

### Recap

So we know how to apply wedge and differentiation operators to differential forms.
Then, we get a number from a differentiation form by integrating it.

### Objective

Both 1-forms and 2-forms correspond to basis vectors in $\mathbb{R}^3$. 1-forms are componenty; 2-forms are surfacey.
The question: *How?*

To answer this question, we have to know differential forms more than as "mathematical objects."

A differential forms is a *function*. 
- takes in vectors 
- outputs a function (which we treat as a number) 

An n-form takes in n vectors.



### Definition: 1-form as a function that takes in 1 vector

There are 3 options + 1 example to explain what this function does. 


##### Option 1. Formula. 

Formula left hand side:
[image]

Formula right hand side:
$$a_k.$$


The $dx_k$ function picks out the $k$th component in its input.



##### Option 2. I tell you this function is linear. I give you its values for the set of basis vectors. 

Every $dx_k$ is linear.

What happens when $dx_k$ takes in a unit vector:
[image]


##### Option 3. This function is a projection.

$dx_k$ means projection onto $e_k$.

$dx_k(\mathbf{v})$ is the $k$th component of $\mathbf{v}$. 


##### Option 4 (Example). Find $dx_1(<8,15,17>)$. Ans: $8$.

Find $dx_2(<8,15,17>)$. Ans: $15$.

Find $dx_3(<8,15,17,1>)$. Ans: $17$.

Find $dx_4(<8,15,17,1>)$. Ans: $1$.


### Answer: 1-forms are component-y basis elements.

Let $\vec{P} = x \; \hat{e_1} + y \; \hat{e_2} + z \; \hat{e_3}$ be a vector in $\mathbb{R}^3$.



### Definition: 2-form as a function that takes in 2 vectors.

3 options + 3 examples to explain what this function does. 

##### Option 1. 