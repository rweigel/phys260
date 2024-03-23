```mdextension
Title: Cross Products
```

# Introduction

The cross product of two vectors $\bfvec{v}$ and $\bfvec{B}$, written as $\bfvec{v}\times\bfvec{B}$, is a vector quantity with a magnitude of $|\bfvec{v}||\bfvec{B}|\sin\phi = vB\sin\phi$, where $\phi$ is the angle between the two vectors ($0 \le\phi \le 180^{\circ}$). The direction of $\bfvec{v}\times\bfvec{B}$ is perpendicular to the plane that contains both vectors. (There are two perpendicular directions, and the one to choose is determined using the cross--product right--hand rule; see your textbook for details.)

Three methods are commonly used for computing a cross product. The first method is useful for certain simple problems, whereas the last two methods apply to all problems.

# The Circle Diagram

Computing the cross--product of two vectors typically involves the cross-products of unit vectors. Unit vector cross products can be determined using the right--hand rule. However, some students find it easier to use a non--visual approach, which is described here. The possible cross products of unit vectors are

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

There is a mnemonic (memory) device for remembering the second and third rows of this table.

* If two unit vectors are crossed, the result is $\pm$, the unit vector not involved in the cross product.

* To determine the sign, connect the two unit vectors that are crossed by drawing the shortest line that connects the first to the second along the circle shown below.

* If the line drawn was clockwise, the cross product is positive. If the line drawn was negative, the cross product is negative.

<img src="../Cross_Products/figures/Cyclic_ijk.svg" width="30%">

## Examples

* The cross product of $\jhat \times \khat$ requires drawing a clockwise line from $\jhat$ to $\khat$, so the result must be positive; the unit vector that was not a part of the cross--product is $\ihat$. Thus $\jhat \times \khat = \ihat$.

* The cross product of $\jhat \times \ihat$ requires drawing a counterclockwise line from $\jhat$ to $\ihat$, so the result must be negative; the unit vector that was not a part of the cross--product is $\khat$. Thus $\jhat \times \ihat = -\khat$.

## Problems

Use the right--hand rule to determine the following cross--products. Then use the circle diagram to check your answer.

\ifsolutions
**Answer**:
A. $\khat \times \ihat = \boxed{\phantom{-}\jhat}\qquad$
B. $\khat \times \jhat = \boxed{-\ihat}\qquad$
C. $\ihat \times \khat = \boxed{-\jhat}$
\else
A. $\khat \times \ihat = \fbox{\phantom M}\qquad$
B. $\khat \times \jhat = \fbox{\phantom M}\qquad$
C. $\ihat \times \khat = \fbox{\phantom M}$
\fi

# By Inspection Method

This method is most useful if the angle $\phi$ between the two vectors is given, obvious, or straightforward to compute. There are two possibilities.

1. Both vectors point along different cartesian axis (so that $\phi=90^\circ$). In this case, the magnitude is the product of the vector lengths (which are positive by definition), and the direction is determined using the cross--product right--hand rule or the circle diagram.

   **Examples**:

   * If $\bfvec{v}=2\ihat$ and $\bfvec{B}=3\jhat$, the cross product $\bfvec{v}\times\bfvec{B}=2\ihat\times3\jhat$ has a magnitude 

     $|2\ihat||3\jhat|\sin 90^\circ = 6|\ihat||\jhat|\sin 90^\circ = 6$.

     The direction is $\khat$, which is determined using the right--hand rule on $\ihat\times\jhat$ or the circle diagram.

     Thus, $\bfvec{v}\times\bfvec{B} = 6\khat$

   * If $\bfvec{v}=-2\jhat$ and $\bfvec{B}=3\khat$, the cross product $-2\jhat\times3\khat$ has a magnitude

     $|-2\jhat||3\khat|\sin 90^\circ = 2\cdot 3|\jhat||\khat|\sin 90^\circ = 6$.

     The direction is $-\ihat$, which is determined using the right--hand rule on $-\jhat\times\khat$ or the circle diagram.

     Thus, $\bfvec{v}\times\bfvec{B}=-6\ihat$

2. Both vectors lie in the same coordinate plane. In this case, compute the magnitude using $|\bfvec{v}||\bfvec{B}|\sin\phi$ and the direction using the cross--product right--hand rule or the circle diagram.

   **Examples**:

   *  If $\bfvec{v}=\ihat$ and $\bfvec{B}=\ihat$, the cross product $\bfvec{v}\times\bfvec{B}=\ihat\times\ihat$ is zero because its magnitude is $|\ihat||\ihat|\sin 0 = 1\cdot 1 \cdot 0$.

   * If $\bfvec{v}=\ihat$ and $\bfvec{B}=\ihat+\jhat$, the cross product $\bfvec{v}\times\bfvec{B}= \ihat\times(\ihat+\jhat)$ has a magnitude of $|\ihat||\ihat+\jhat|\sin 45^\circ = 1\cdot \sqrt{2} \sin 45^\circ = 1$

     (From a diagram, it should be straightforward to see that the angle between $\ihat$ and $\ihat+\jhat$ is $45^\circ$ and the magnitude of $\bfvec{B}$ is $\sqrt{2}$).

    The direction is $\khat$, which can be determined using the cross--product right--hand rule. Thus, $\bfvec{v}\times\bfvec{B}=\sqrt{2} \sin 45^\circ\khat = \khat$.

\ifsolutions
\else
\newpage
\fi

## Problems

Compute $\bfvec{v}\times\bfvec{B}$ for each of the following cases.

\ifsolutions
**Answers**:

* $\bfvec{v}=v_x\ihat\quad$ and $\quad\bfvec{B}=\phantom{-}B_y\jhat$, $\quad\bfvec{v}\times\bfvec{B} = \boxed{v_xB_y\khat}$

* $\bfvec{v}=v_x\ihat\quad$ and $\quad\bfvec{B}=-B_y\jhat$, $\quad\bfvec{v}\times\bfvec{B} = \boxed{-v_xB_y\khat}$

* $\bfvec{v}=v_z\khat\quad$ and $\quad\bfvec{B}=\phantom{-}B_y\jhat$, $\quad\bfvec{v}\times\bfvec{B} = \boxed{-v_zB_y\ihat}$

\else
\vspace{5em}

* $\bfvec{v}=v_x\ihat\quad$ and $\quad\bfvec{B}=\phantom{-}B_y\jhat$, $\quad\bfvec{v}\times\bfvec{B} = \fbox{\qquad\phantom M}$

\vspace{5em}

* $\bfvec{v}=v_x\ihat\quad$ and $\quad\bfvec{B}=-B_y\jhat$, $\quad\bfvec{v}\times\bfvec{B} = \fbox{\qquad\phantom M}$

\vspace{5em}

* $\bfvec{v}=v_z\khat\quad$ and $\quad\bfvec{B}=\phantom{-}B_y\jhat$, $\quad\bfvec{v}\times\bfvec{B} = \fbox{\qquad\phantom M}$

\fi

\vspace{3em}

----

Compute $\bfvec{v}\times\bfvec{B}$ based on the information in the following diagrams. Write your answers below each diagram.

<img src="figures/Diagram_I.svg">

\ifsolutions
**a.**
$\quad\bfvec{v}\times\bfvec{B} = 60\sin 30^\circ\khat$

**b.** $\quad\bfvec{v}\times\bfvec{B}=-42\ihat$

**c.** $\quad\bfvec{v}\times\bfvec{B} = \frac{18}{\sqrt{2}}(\ihat - \jhat)$
\else
\newpage
\fi

# Multiply Through Method

This method is most useful when each of the vectors in the cross--product has two or fewer components. Otherwise, the Determinant Method, covered in the next section, is preferred.

Write the vectors in component form and then "multiply through" in a way that is similar to "multiplying through" to convert the product of sums into a sum of products. For example,

$$a(b+c)=(a\cdot b) + (a\cdot c)$$

and the first--outer--inner--last (foil) case

$$(a+b)(c+d)=(a\cdot c) + (a\cdot d) + (b\cdot c) + (b\cdot d)$$

but replace the multiplication symbol ($\cdot$) with the cross product symbol ($\times$).

## Examples

* If $\bfvec{v}=v_x\ihat$ and $\bfvec{B}=B_x\ihat+B_y\jhat$, then

  $$
  \begin{align*}
  \bfvec{v}\times\bfvec{B} &= v_x\ihat\times(B_x\ihat+B_y\jhat)\\
  &= v_xB_x(\ihat\times\ihat) + v_xB_y(\ihat\times\jhat)\\
  &= 0 + v_xB_y\khat = \khat
  \end{align*}
  $$

* If $\bfvec{v}=v_x\ihat$ and $\bfvec{B}=B_x\ihat+B_y\jhat + B_z\khat$, then

  $$
  \begin{align*}
  \bfvec{v}\times\bfvec{B} &= v_x\ihat\times(B_x\ihat+B_y\jhat+B_z\khat) \\
  & = v_xB_x(\ihat\times\ihat) + v_xB_y(\ihat\times\jhat) + v_xB_z(\ihat\times\khat)\\
  & = 0 + v_xB_y\khat - v_xB_z\jhat
  \end{align*}
  $$

\ifsolutions
\else
\newpage
\fi

## Problems

Use the "Multiply Through" method for these problems.

Compute $\bfvec{v}\times\bfvec{B}$ and write your answer after the equal sign for each of the following cases.

\ifsolutions
* $\bfvec{v}=v_x\ihat+v_y\jhat+v_z\khat\quad$ and $\quad\bfvec{B}=B_x\ihat$, $\quad\bfvec{v}\times\bfvec{B} = \boxed{-v_yB_x\ihat+v_zB_x\jhat}$
\else
\vspace{4em}
* $\bfvec{v}=v_x\ihat+v_y\jhat+v_z\khat\quad$ and $\quad\bfvec{B}=B_x\ihat$, $\quad\bfvec{v}\times\bfvec{B} = \fbox{\qquad\qquad\qquad\phantom M}$
\fi


\ifsolutions
* $\bfvec{v}=v_x\ihat+v_y\jhat\quad$ and $\quad\bfvec{B}=B_x\ihat+B_y\jhat$, $\quad\bfvec{v}\times\bfvec{B} = \boxed{(v_xB_y-v_yB_x)\khat}$
\else
\vspace{4em}
* $\bfvec{v}=v_x\ihat+v_y\jhat\quad$ and $\quad\bfvec{B}=B_x\ihat+B_y\jhat$, $\quad\bfvec{v}\times\bfvec{B} = \fbox{\qquad\qquad\qquad\phantom M}$
\fi

----

Compute $\bfvec{v}\times\bfvec{B}$ based on the information in the following diagrams by writing $\bfvec{v}$ and $\bfvec{B}$ in vector notation and using the Multiply Through Method. Show your work in the space below each diagram.

<img src="figures/Diagram_I.svg">

\ifsolutions
**a.**

$\quad\bfvec{v}=10\cos 45^\circ\ihat + 10\sin 45^\circ\jhat$

$\quad\bfvec{B}=6\cos 15^\circ\ihat + 6\sin 15^\circ\jhat$

$$
\begin{align*}
\quad\bfvec{v}\times\bfvec{B} &= (10\cos 45^\circ \cdot 6\sin 15^\circ-10\sin 45^\circ \cdot 6\cos 15^\circ)\khat\\
&= 60\sin 30^\circ\khat
\end{align*}
$$

$\quad$where the last equality follows from a trig identity.

**b.**

$\quad\bfvec{v}\times\bfvec{B} = 7\khat \times (6\jhat + 7\khat) = -42\ihat$

**c.**

$\quad\bfvec{v}\times\bfvec{B} = \frac{3}{\sqrt{2}}(\ihat+\jhat)\times 6\khat = \frac{18}{\sqrt{2}}(\ihat - \jhat)$
\else
\newpage
\fi

# Determinant Method

To find all non--zero terms that would have resulted using the Determinant Method, write the cross product in matrix determinant form as follows and compute its determinant. (This requires that you have memorized the procedure for computing the determinant of a $3\times 3$ matrix.) The most general problem and steps are as follows.

$$
\begin{align*}
\bfvec{v}\times\bfvec{B}
&=
\begin{vmatrix}
\ihat&\jhat&\khat\\
v_x&v_y&v_z\\
B_x&B_y&B_z\\
\end{vmatrix}
\\\\ &=
\begin{vmatrix}
v_y & v_z \\
B_y & B_z 
\end{vmatrix} \ihat - \begin{vmatrix}
v_x & v_z \\
B_x & B_z 
\end{vmatrix} \jhat +  \begin{vmatrix}
v_x & v_y \\
B_x & B_y 
\end{vmatrix} \khat
\\\\ &=
(v_yB_z - v_zB_y)\ihat -(v_xB_z - v_zB_x)\jhat +(v_xB_y - v_yB_x)\khat
\end{align*}
$$

## Example

If $\bfvec{v}=2\ihat$ and $\bfvec{B}=3\ihat+4\jhat$, then

$$
\begin{align*}
\bfvec{v}\times\bfvec{B}
&=
\begin{vmatrix}
\ihat&\jhat&\khat\\
2&0&0\\
3&4&0\\
\end{vmatrix}
\\\\ &=
\begin{vmatrix}
0 & 0 \\
4 & 0 
\end{vmatrix} \ihat - \begin{vmatrix}
2 & 0 \\
3 & 0 
\end{vmatrix} \jhat +  \begin{vmatrix}
2 & 0 \\
3 & 4 
\end{vmatrix} \khat
\\\\ &=
0\ihat - 0\jhat + 8\khat
\end{align*}
$$

(One could have used the general formula given above, but here we assume you don't have it memorized.)

## Problem

If $\bfvec{v}=1\ihat+2\jhat$ and $\bfvec{B}=3\ihat+4\jhat$, use the Determinant Method to find $\bfvec{v}\times\bfvec{B}$. Show your work.

\ifsolutions

$$
\begin{align*}
\bfvec{v}\times\bfvec{B}
&=
\begin{vmatrix}
\ihat&\jhat&\khat\\
1&2&0\\
3&4&0\\
\end{vmatrix}
\\ &=
\begin{vmatrix}
2 & 0 \\
4 & 0 
\end{vmatrix} \ihat - \begin{vmatrix}
1 & 0 \\
3 & 0 
\end{vmatrix} \jhat +  \begin{vmatrix}
1 & 2 \\
3 & 4 
\end{vmatrix} \khat
\\ &=
0\ihat - 0\jhat + (4-6)\khat
\\ &=
-2\khat
\end{align*}
$$

\fi