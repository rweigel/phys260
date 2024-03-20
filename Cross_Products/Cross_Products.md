# Introduction

The cross product of two vectors $\bfvec{v}$ and $\bfvec{B}$ is given by $\bfvec{v}\times\bfvec{B}$, which is a vector quantity with a magnitude of $vB\sin\phi$, where $\phi$ is the angle between the two vectors. The direction of $\bfvec{v}\times\bfvec{B}$ is perpendicular to the plane that contains both vectors. (There are two perpendicular directions, and the one to choose is determined using the cross--product right--hand rule; see your textbook of this right--hand rule.)

There are two methods that are commonly used for computing a cross product.

## Method I

If the angle $\phi$ is given or straightforward to compute and both vectors (a) lie in a coordinate plane or (b) both vectors point along a cartesian axis, the magnitude is given by $|\bfvec{v}||\bfvec{B}|\sin\phi$ and the direction of the cross product can be determined using the cross--product right--hand rule.

Examples of case (a): 

* The cross product of $\ihat\times\ihat$ is zero because its magnitude is $|\ihat||\ihat|\sin 0 = 1\cdot 1 \cdot 0$.
* The cross product of $\ihat$ and $\ihat+\jhat$ has a magnitude of $|\ihat||\ihat+\jhat|\sin 45^\circ = 1\cdot \sqrt{2} \cdot 1/\sqrt{2}=1$. (From a diagram, it is straightforward to see that the angle between $\ihat$ and $\ihat+\jhat$ is $45^\circ$). The direction $\khat$, which can be determined using the cross--product right--hand rule or the method using the circle diagram described in the following section.

Example of case (b):
   
* The cross product $2\ihat\times3\jhat$ has a magnitude $|2\ihat||3\jhat|\sin 90^\circ = 6$. The direction is $\khat$, which is determined using the right--hand rule.


## Method II

Write the vectors in component form and then use either the (a) "multiply through" or (a) "determinant" method.

**"Multiply through" method**:
   
Re--write $(v_x\ihat + v_y\jhat + v_z\khat)\times (B_x\ihat + B_y\jhat + B_z\khat)$ as 9 cross products (3 of which will be zero) and evaluate each of the six cross products.

Example:

$(v_x\ihat + v_y\jhat)\times (B_x\ihat + B_y\jhat) = v_xB_x(\ihat\times\ihat) + v_xB_y(\ihat\times\jhat)  + v_yB_x(\jhat\times\ihat) + v_yB_y(\jhat\times\jhat)$

The first and last terms are zero because $\ihat\times\ihat=0$ and $\jhat\times\jhat=0$. Using the right--hand rule or the circle diagram described in the following setion, $\ihat\times\jhat=\khat$ and $\jhat\times\ihat=-\khat$. This leaves

$(v_x\ihat + v_y\jhat)\times (B_x\ihat + B_y\jhat) = (v_xB_y-v_yB_x)\khat$

**"Determinant method"**:

To determine all non--zero terms that would have resulted using the "multiply through" method, write the cross product in matrix form and compute the determinant.

$$
\bfvec{v}\times\bfvec{B} =
\begin{bmatrix}
\ihat&\jhat&\khat\\
v_x&v_y&v_z\\
B_x&B_y&B_z\\
\end{bmatrix}
= (v_yB_z - v_zB_y)\ihat -(v_xB_z - v_zB_z)\jhat +(v_xB_y - v_yB_x)\khat
$$

# Unit Vector Cross--Products

Computing the cross product of two vectors typically involves computation of cross products of unit vectors. The possible cross--products of unit vectors are

$$
\begin{align*}
\ihat\times\ihat & = \phantom{-}0 \qquad &
\jhat\times\jhat & = \phantom{-}0 \qquad &
\khat\times\khat & = \phantom{-}0 \qquad
\\
\ihat\times\jhat & =  \phantom{-}\khat &
\jhat\times\khat & = \phantom{-}\ihat  &
\khat\times\ihat & = \phantom{-}\jhat
\\
\jhat\times\ihat & = -\khat &
\khat\times\jhat & = -\ihat &
\ihat\times\khat & = -\jhat
\end{align*}
$$

There is a mnemonic (memory) device for remembering this table. Suppose you do the cross product of two consecutive unit vectors in the order indicated by the arrows in the circle shown in the following figure. In that case, the result is the remaining unit vector (the second row in the table). If you do the cross product of two unit vectors in reverse order, the result is the remaining unit vector with a negative sign (the third row in the table).

<img src="../Cross_Products/figures/Cyclic_ijk.svg"/>

Example: The cross product of $\jhat \times \ihat$ requires going counterclockwise from $\jhat$ in the circle to $\ihat$, so the result must be negative; the direction must be the unit vector that was not a part of the cross--product, which is $\khat$. Thus $\jhat \times \ihat = -\khat$.

# Problems

## Method 1.

Use Method I described in the introduction for these problems.

Compute $\bfvec{v}\times\bfvec{B}$ and write your answer after the equal sign for each of the following cases.

* $\bfvec{v}=v_x\ihat$ and $\bfvec{B}=B_y\jhat$, $\bfvec{v}\times\bfvec{B} =$
* $\bfvec{v}=v_x\ihat$ and $\bfvec{B}=-B_x\jhat$, $\bfvec{v}\times\bfvec{B} =$
* $\bfvec{v}=v_y\ihat$ and $\bfvec{B}=B_z\jhat$, $\bfvec{v}\times\bfvec{B} =$

Compute $\bfvec{v}\times\bfvec{B}$ based on the information in the following diagrams.

1. 

2. 

3. 

## Method II

Use Method II described in the introduction for these problems (which are identical to the previous problems).

Compute $\bfvec{v}\times\bfvec{B}$ and write your answer after the equal sign for each of the following cases.

* $\bfvec{v}=v_x\ihat$ and $\bfvec{B}=\phantom{-}B_y\jhat$, $\bfvec{v}\times\bfvec{B} =$
* $\bfvec{v}=v_x\ihat$ and $\bfvec{B}=-B_x\jhat$, $\bfvec{v}\times\bfvec{B} =$
* $\bfvec{v}=v_y\ihat$ and $\bfvec{B}=\phantom{-}B_z\jhat$, $\bfvec{v}\times\bfvec{B} =$

Compute $\bfvec{v}\times\bfvec{B}$ based on the information in the following diagrams.

1. 

2. 

3. 
