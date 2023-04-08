# Cross product review

Thus far, only the cross product of vectors with one component were considered, e.g.,

$$\bfvec{v} \times \bfvec{B} = v_o\ihat \times B_o\jhat$$

The most general case that you will encounter is

$$\mathbf{v}\times \mathbf{B} = (v_x\ihat + v_y\jhat + v_z\khat)\times (B_x\ihat + B_y\jhat + B_z\khat)$$

which has a cross product of 

$$\mathbf{v}\times \mathbf{B} = (v_yB_z - v_zB_y)\ihat + (v_zB_x - v_xB_z)\jhat + (v_xB_y - v_yB_x)\khat$$

This formula is not easy to memorize. There are two ways to derive it

1. Using the "determinant method": https://www.youtube.com/watch?v=2wTUqZa66ng
2. By splitting up  $(v_x\ihat + v_y\jhat + v_z\khat)\times (B_x\ihat + B_y\jhat + B_z\khat)$ into 9 cross products (3 of which will be zero).

When the number of components in $\bfvec{v}$ and $\bfvec{B}$ is two or less, I recommend using method 2.

## Example

As an example of method 2., consider the case

$$(v_x\ihat)\times (B_x\ihat + B_y\jhat + B_z\khat)$$

This can be re-written as (by doing the equivalent of "multiplying through")

$$(v_x\ihat\times B_x\ihat) + (v_x\ihat\times B_y\jhat) + (v_x\ihat\times B_z\khat)$$

After factoring out the constants, this is

$$v_xB_x(\ihat\times \ihat) + v_xB_y(\ihat\times \jhat)+ v_xB_z(\ihat\times \khat)$$

The first term is zero because $\ihat\times\ihat=0$. The second term  is $v_xB_y\khat$ because $\ihat \times\jhat = \khat$. The third term is $-v_xB_z\jhat$ because $\ihat\times\khat=-\jhat$. Thus,

$$(v_x\ihat)\times (B_x\ihat + B_y\jhat + B_z\khat)=-v_xB_y\jhat + v_xB_y\khat$$

## Problems

1. Use method 2. to find $(v_y\jhat)\times (B_x\ihat + B_y\jhat + B_z\khat)$

2. Use method 2. to find $(v_x\ihat + v_y\jhat)\times (B_x\ihat + B_y\jhat)$

\ifsolutions
**Answer**

1. $(v_y\jhat)\times (B_x\ihat + B_y\jhat + B_z\khat)=v_yB_x\jhat\times\ihat + v_yB_y\jhat\times\jhat + v_yB_z\jhat\times\khat$. The middle term is zero, leaving

  $v_yB_x\jhat\times\ihat + v_yB_z\jhat\times\khat= v_yB_z\ihat-v_yB_x\khat$

2. $(v_x\ihat + v_y\jhat)\times (B_x\ihat + B_y\jhat) = v_xB_y\ihat\times\jhat + v_yB_x\jhat\times\ihat$ (The two terms that involve $\ihat\times\ihat$ and $\jhat\times\jhat$ have been omitted.). This leaves

  $v_xB_y\khat - v_yB_x\khat=(v_xB_y - v_yB_x)\khat$

\else
\fi