Right now, these notes connect with prior knowledge described in [Recap] in order to answer [Objective] and are written in Obsidian md. They will later grow independent and become html. Before that, please see `.pdf` of obsidian looks.

# differential-forms-in-chalk

## Recap

So we know how to apply wedge and differentiation operators to differential forms.
Then, we get a number from a differentiation form by integrating it.

## Objective

Both 1-forms and 2-forms correspond to basis vectors in $\mathbb{R}^3$. 1-forms are componenty; 2-forms are surfacey.
The question: *How?*

To answer this question, we have to know differential forms more than as "mathematical objects."

A differential forms is a *function*. 
- takes in vectors 
- outputs a function (which we treat as a number) 

An n-form takes in n vectors.



## Definition: 1-form as a function that takes in 1 vector

There are 3 options + 1 example to explain what this function does. 


### Option 1. Formula. 

Formula left hand side:
![[Pasted image 20230107222747.png | 400]]

Formula right hand side:
$$a_k.$$


The $dx_k$ function picks out the $k$th component in its input.



### Option 2. I tell you this function is linear. I give you the base cases.

Every $dx_k$ is a linear function.

What happens when each $dx_k$ takes in a unit vector:
![[Pasted image 20230107223023.png | 400]]


### Option 3. This function is a projection.

$dx_k$ means projection onto $e_k$.

$dx_k(\mathbf{v})$ is the $k$th component of $\mathbf{v}$. 


### Note following options 1, 2, 3.

If we want to find $\omega(\mathbf{v})$ where $\omega$ is not a basis 1-form $(\omega = dx_k)$ but a linear combination of basis 1-forms,
$$
\omega = \sum_i c_i \; dx_i,
$$
then 
$$
\omega(\mathbf{v}) = \sum_i c_i \; dx_i(\mathbf{v}).
$$


### Option 4 (Example). Find $dx_1(<8,15,17>)$. Ans: $8$.

Find $dx_2(<8,15,17>)$. 
> Ans: $15$.

Find $dx_3(<8,15,17,1>)$.
> Ans: $17$.

Find $dx_4(<8,15,17,1>)$. 
> Ans: $1$.

Find $\omega(<8,15,17>)$ where $\omega = dx_1 +dx_2$.
> Ans: $8 + 15 = 23$

Find $\omega(<8,15,17>)$ where $\omega = 3 \; dx_1 + 7 \; dx_2$.
> Ans: $3\cdot 8 + 7\cdot 15 = 129$



## Answer: 1-forms are component-y basis elements.

### Dictionary

![[Pasted image 20230107223144.png | 400]]

### The associated 1-form of a vector is called its "work form."

![[Pasted image 20230107223232.png | 400]]

Reiterate: 
If $\omega$ is the work form (1-form counterpart) of $\mathbf{x}$, then
$$
\mathbf{x} \cdot \mathbf{u} = \omega(\mathbf{u}).
$$

## Definition: 2-form as a function that takes in 2 vectors.

3 options + 3 examples to explain what this function does. 

### Option 1. Formula.

Formula left hand side:
![[Pasted image 20230107223741.png | 400]]

Formula right hand side:
![[Pasted image 20230107223848.png | 400]]

This function is a determinant.
We rely on a matrix of 1-forms acting on 1 vector.


#### Mnemonics

- For a matrix to be determinant-able, it has to be square.
		![[Pasted image 20230107223933.png | 400]]
	Thus 2-forms require 2 vectors for input.
	
- If there are identical rows, the determinant is $0$.
	For $\omega = dx_k \wedge dx_k$,

$$
\omega(\vec{u},\vec{v}) = \begin{pmatrix}
u_k & v_k \\
u_k & v_k
\end{pmatrix},
$$
	so it has identical rows.


### Option 2. Generalize a linear function to take more than 1 input.

If we add an input, we can go from *linear* to *multilinear*.
[image relating with determinant properties]
- vector addition:
- scalar multiplications:

When there are multiple inputs, should the order of inputs matter?
Yes:
$$
\omega(\mathbf{u},\mathbf{v}) = - \omega(\mathbf{u},\mathbf{v}).
$$
The sign is alternated when the order of two inputs is switched. This flavour of "order matters" is called *alternating*.

In summary, the 2-form is an *multilinear alternating* function. (Make your own base cases from the formula given option 1.)


### Option 3. This function is a projection.

$dx_i \wedge dx_j$ means projection onto the plane spanned by $e_i, \; e_j$.

$dx_i \wedge dx_j(\mathbf{u}, \mathbf{v})$ is the area of the parallelogram spanned by the projections of $\mathbf{u}, \mathbf{v}$ onto $e_i, \; e_j$.


### Option 4 (Example). Find $dx_1 \wedge dx_2 (<8,15,17>, <3,4,5>)$. Ans: $-13$.


## Answer: 2-forms are component-y basis elements.

### Dictionary
[image]

### The associated 2-form of a vector is called its "flux form."
[image]