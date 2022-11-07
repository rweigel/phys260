```mdextension
Title: Lorentz Force
```

# Introduction

Charges create an electric field. The charges that create the electric field can be stationary or moving.

A stationary or moving charge $q$ in an electric field (created by other charges) experiences a force of

$$\bfvec{F} = q\bfvec{E}$$

A magnetic field is created by moving charges. A stationary charge {\it does not} create a magnetic field. A moving charge $q$ in a magnetic field (created by other moving charges) experiences a force of

$$\bfvec{F} = q\bfvec{v}\times\bfvec{B}$$

The direction of the force on $q$ is perpendicular to a plane that contains $\bfvec{v}$ and $\bfvec{B}$. This plane can be visualized by imagining orienting a piece of paper such that both the  $\bfvec{v}$ and $\bfvec{B}$ vectors lie on the paper. See Figure 27.6 of the textbook.

The magnitude of $\bfvec{F}$ can be computed using the above equation or

$$F = qvB\sin\phi$$

where $\phi$ is the angle between $\bfvec{v}$ and $\bfvec{B}$ and $\phi \le 180^{\circ}$. (For example, the angle between two vectors can be said to be $10^{\circ}$ or $350^{\circ}$. In the above equation, use $10^{\circ}$ -- if $350^{\circ}$ was used, we would get a negative value for the magnitude of $F$, which is positive by definition because it is a magnitude.)

There are two special cases for which the general equation $\bfvec{F} = q\bfvec{v}\times\bfvec{B}$ simplifies to a very simple equation:

1. If the direction of motion is perpendicular to the magnetic field (so that $\phi = 90^{\circ}$), the magnitude of the force is $F = qvB$ and the direction is determined by right-hand-rule.
2. If the direction of motion is parallel or anti-parallel to the magnetic field (so that $\phi = 0^{\circ}$ or $\phi = 180^{\circ}$), the magnitude of the force is $F = 0$.

# Calculating Forces

## Simple Case

When the vectors in a cross product are in a cartesian coordinate plane (so that the angle between them is easily computed) the formula $F = qvB\sin\phi$ can be used to find the magnitude of $F$ and the direction is given by the right--hand rule.

When the vectors are not in a coordinate plane, finding the angle between them is require a diagrame and several steps of trigonometry. In this case, it is easier to use vector notation to compute the cross product.

## Computing $\bfvec{F}$ and $F$ Using Vector Notation

The calculation of the cross product when both vectors in the cross product are along one of the Cartesian coordinate axes is the easiest case (e.g., $\bfvec{B}=B_o\ihat$ and $\bfvec{v}=v_o\jhat$). There are two ways of determining the cross-product in this case:

1. visually by using the right-hand-rule with the two unit vectors as was done in Section 2.1; and
2. by using the following table of cross products.

  $$
  \begin{align*}
  \ihat\times\ihat &  = 0  & \jhat\times\jhat & =0  &   \khat\times\khat & = 0 \\
  \ihat\times\jhat & = \khat  & \jhat\times\khat & = \ihat  & \khat\times\ihat & =  \jhat \\
   \jhat\times\ihat & =-\khat & \khat\times\jhat &  = -\ihat & \ihat\times\khat & = -\jhat \\
   \end{align*}
   $$

There is a mnemonic (memory) device for remembering this table. If you do the cross product of two consecutive unit vectors in the order indicated by the arrows in the circle shown in the following figure, the result is the remaining unit vector (the second row in the table). If you do the cross product of two unit vectors in reverse order, the result is the remaining unit vector with a negative sign (the third row in the table).

<img src="figures/Cyclic.svg"/>

# Example

<img src="figures/Lorentz_Force.svg"/>

For case f. in the figure above,

1. write a vector equation for both $\bfvec{v}$ and $\bfvec{B}$ and use them to compute the force vector using $\bfvec{F} = q\bfvec{v}\times\bfvec{B}$ assuming that $\bfvec{B}=B_o\ihat$ and $|\bfvec{v}|=v_o$. Then compute the magnitude of $\bfvec{F}$. Verify that the vector direction of $\bfvec{F}$ is consistent with what you expect from using the right-hand-rule; 
2. use $F = qvB\sin\phi$ to compute the magnitude of the force and verify that you get the same magnitude. 

{\bf f.1} $\bfvec{v}=-v_o\khat$, so $\bfvec{F} = q(-v_o\khat)\times (B_o\ihat)=-qv_oB_o(\khat\times \ihat)=-qv_oB_o\jhat$; $|\bfvec{F}|=qv_oB_o$.

{\bf f.2} $\phi=90^{\circ}$, so $F = qv_oB_o\sin(90^{\circ})=qv_oB_o$.

\newpage

# Problem

Answer questions 1. and 2. given in the previous problem for cases a.-e. in the figure above. Assume that the magnitude of the velocity is $v_o$ and the magnitude of the magnetic field is $B_o$.

{\bf a.1}
\ifsolutions
$\bfvec{v}=v_o\jhat$, so $\bfvec{F} = q\,(v_o\jhat)\times (B_o\ihat)=qv_oB_o(\jhat\times \ihat)=-qv_oB_o\khat$; $|\bfvec{F}|=qv_oB_o$
\else
<div style="height:3em"/>
\fi

{\bf a.2}
\ifsolutions
$\theta=90^{\circ}$, so $F = qv_oB_o\sin(90^{\circ})=qv_oB_o$.
\else
<div style="height:3em"/>
\fi

{\bf b.1}
\ifsolutions
$\bfvec{v}=-v_o\jhat$, so $\bfvec{F} = -q\,(v_o\jhat)\times (B_o\ihat)=qv_oB_o(\jhat\times \ihat)=qv_oB_o\khat$; $|\bfvec{F}|=qv_oB_o$
\else
<div style="height:3em"/>
\fi
{\bf b.2}
\ifsolutions
$\theta=90^{\circ}$, so $F = qv_oB_o\sin(90^{\circ})=qv_oB_o$.
\else
<div style="height:3em"/>
\fi

{\bf c.1}
\ifsolutions
$\bfvec{v}=-v_o\ihat$, so $\bfvec{F} = -q\,(v_o\ihat)\times (B_o\ihat)=-qv_oB_o(\jhat\times \ihat)=0$; $|\bfvec{F}|=0$
\else
<div style="height:3em"/>
\fi

{\bf c.2}
\ifsolutions
$\theta=90^{\circ}$, so $F = qv_oB_o\sin(180^{\circ})=0$.
\else
<div style="height:3em"/>
\fi

{\bf d.1}
\ifsolutions
$\bfvec{v}=v_o\ihat$, so $\bfvec{F} = q\,(v_o\ihat)\times (B_o\ihat)=qv_oB_o(\ihat\times \ihat)=0$; $|\bfvec{F}|=0$
\else
<div style="height:3em"/>
\fi

{\bf d.2}
\ifsolutions
$\theta=90^{\circ}$, so $F = qv_oB_o\sin(0^{\circ})=0$.
\else
<div style="height:3em"/>
\fi

{\bf e.1}
\ifsolutions
$\bfvec{v}=v_o\khat$, so $\bfvec{F} = q\,(v_o\khat)\times (B_o\ihat)=qv_oB_o(\khat\times \ihat)=qv_oB_o\jhat$; $|\bfvec{F}|=qv_oB_o$
\else
<div style="height:3em"/>
\fi

{\bf e.2}
\ifsolutions
$\theta=90^{\circ}$, so $F = qv_oB_o\sin(90^{\circ})=qv_oB_o$.
\else
%\vspace{0.35in}
\fi

\newpage

# Trajectories

Previously, you computed the force on a moving charged particle in a magnetic field.

As the particle moves, its velocity vector changes. As a result, the direction of force changes. This behavior was addressed when the forces on curved wire segments were computed.

A charged particle moving through a magnetic field will tend to rotate in a circle around the magnetic field lines. There are three general trajectories:

1. The velocity is parallel to the magnetic field lines. In this case, the particle will continue to move in a straight line because no magnetic forces are acting on it.
2. The velocity is perpendicular to the magnetic field lines. In this case, the particle motion will be a circle in the same plane as the velocity vector.
3. The velocity has components that are both parallel and perpendicular to the magnetic field line. In this case, the particle will move at a constant velocity in the direction of the field line and move in a circle around the field line. The path of the particle will be a spiral.

## Problem

Use the simulation at https://ophysics.com/em8.html to verify the above statements. Comment here on how you simulated each of these and what they showed. 

1.
<div style="height:3em"/>

2.
<div style="height:3em"/>

3.

<div style="height:3em"/>

\newpage

# Cross product review

Thus far, only the cross product of vectors with one component were considered, e.g.,

$$\bfvec{v} \times \bfvec{B} = v_o\ihat \times B_o\yhat$$

The most general case that you will encounter is

$$\mathbf{A}\times \mathbf{B} = (A_x\ihat + A_y\jhat + A_z\khat)\times (B_x\ihat + B_y\jhat + B_z\khat)$$

which has a cross product of 

$$\mathbf{A}\times \mathbf{B} = (A_yB_z - A_zB_y)\ihat + (A_zB_x - A_xB_z)\jhat + (A_xB_y - A_yB_x)\khat$$

This formula is not easy to memorize. There are two ways to derive it

1. Using the "determinant method": https://www.youtube.com/watch?v=2wTUqZa66ng
2. By splitting up  $(A_x\ihat + A_y\jhat + A_z\khat)\times (B_x\ihat + B_y\jhat + B_z\khat)$ into 9 cross products (3 of which will be zero).

When the number of components in $\bfvec{A}$ and $\bfvec{B}$ is two or less, I recommend using method 2.

## Example

As an example of 2., consider the case

$$(A_x\ihat)\times (B_x\ihat + B_y\jhat + B_z\khat)$$

This can be re-written as (by doing the equivalent of "multiplying through")

$$(A_x\ihat\times B_x\ihat) + (A_x\ihat\times B_y\jhat) + (A_x\ihat\times B_z\khat)$$

After factoring out the constants, this is

$$A_xB_x(\ihat\times \ihat) + A_xB_y(\ihat\times \jhat)+ A_xB_z(\ihat\times \khat)$$

The first term is zero because $\ihat\times\ihat=0$. The second term  is $A_xB_y\khat$ because $\ihat \times\jhat = \khat$. The third term is $-A_xB_z\jhat$ because $\ihat\times\khat=-\jhat$. Thus,

$$(A_x\ihat)\times (B_x\ihat + B_y\jhat + B_z\khat)=-A_xB_y\jhat + A_xB_y\khat$$

## Problems

1. Use method 2. to find $(A_y\jhat)\times (B_x\ihat + B_y\jhat + B_z\khat)$

2. Use method 2. to find $(A_x\ihat + A_y\jhat)\times (B_x\ihat + B_y\jhat)$
