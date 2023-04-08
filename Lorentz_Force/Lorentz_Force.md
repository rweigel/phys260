```mdextension
Title: Lorentz Force
```

# Introduction

A stationary or moving charge $q$ in an electric field (created by other charges) experiences a force of

$$\bfvec{F} = q\bfvec{E}$$

A moving charge creates a magnetic field. A moving charge $q$ in a magnetic field (created by other moving charges) experiences a force of

$$\bfvec{F} = q\bfvec{v}\times\bfvec{B}$$

The direction of the force on $q$ is perpendicular to a plane that contains $\bfvec{v}$ and $\bfvec{B}$. This plane can be visualized by imagining orienting a flat piece of paper such that both the  $\bfvec{v}$ and $\bfvec{B}$ vectors lie on the paper. The direction of $\bfvec{v}\times\bfvec{B}$ is perpendicular to the paper. As discussed in the Electric Flux activity, there are two perpendicular directions for a plane; the one to choose is determined by the right--hand rule for cross products.

The magnitude of $\bfvec{F}$ can be computed using the above equation to find $F_x$, $F_y$, and $F_z$ and then $F=\sqrt{F_x^2+F_y^2+F_z^2}$. Or, one can use

$$F = |q|vB\sin\phi\thinspace,$$

where $\phi$ is the angle between $\bfvec{v}$ and $\bfvec{B}$ and $0 \le\phi \le 180^{\circ}$. (For example, the angle between two vectors can be said to be $\phi=10^{\circ}$ or $\phi=350^{\circ}$. In the above equation, use $10^{\circ}$; if $350^{\circ}$ was used, you would get a negative value for the magnitude of $F$, which is positive by definition because it is a magnitude.)

There are two special cases for which the general equation $\bfvec{F} = q\bfvec{v}\times\bfvec{B}$ simplifies to a very simple equation:

1. If the direction of motion of $q$ is perpendicular to the magnetic field (so that $\phi = 90^{\circ}$), the magnitude of the force is $F = qvB$ and the direction of $F$ is determined by the right--hand rule.
2. If the direction of motion is parallel or antiparallel to the magnetic field (so that $\phi = 0^{\circ}$ or $\phi = 180^{\circ}$), the magnitude of the force is zero.

When the vectors in a cross product are both in a Cartesian coordinate plane (so that the angle $\phi$ between them is easily computed), the formula $F = |q|vB\sin\phi$ can be used to find the magnitude of $F$ and its direction is given by the right--hand rule. Otherwise, finding the angle $\phi$ and the perpendicular direction requires a diagram and several steps of trigonometry. In this case, using vector notation to compute $\bfvec{F}$ is easier.

\newpage

# Calculating Forces

In this section, you will compute the magnitude and direction of the force in two ways: 1. using $F = |q|vB\sin\phi$ and the cross--product right--hand rule and 2. using vector notation to find $\bfvec{F}=q\bfvec{v}\times\bfvec{B}$ in component form and then computing the magnitude $|\bfvec{F}|$. 

The problems given are most easily solved using the first method. You are also asked to solve the problems using the second method as preparation for problems that are more easily solved this way.

## Computing $\bfvec{F}$ and $F$ Using Vector Notation

The calculation of the cross product when both vectors in the cross product are along one of the Cartesian coordinate axes is the easiest case (e.g.,  $\bfvec{v}=v_o\jhat$ and $\bfvec{B}=B_o\ihat$). There are two ways of determining the cross--product $\bfvec{v}\times\bfvec{B}$ in this case:

1. using the right--hand rule with the two unit vectors to determine the direction of $\bfvec{F}$ and $|q|vB$ for the magnitude of $F$ or
2. using $q\bfvec{v}\times\bfvec{B}$ and the following table of cross products.

  $$
  \begin{align*}
  \ihat\times\ihat &  = 0  & \jhat\times\jhat & =0  &   \khat\times\khat & = 0 \\
  \ihat\times\jhat & = \khat  & \jhat\times\khat & = \ihat  & \khat\times\ihat & =  \jhat \\
   \jhat\times\ihat & =-\khat & \khat\times\jhat &  = -\ihat & \ihat\times\khat & = -\jhat \\
   \end{align*}
   $$

There is a mnemonic (memory) device for remembering this table. Suppose you do the cross product of two consecutive unit vectors in the order indicated by the arrows in the circle shown in the following figure. In that case, the result is the remaining unit vector (the second row in the table). If you do the cross product of two unit vectors in reverse order, the result is the remaining unit vector with a negative sign (the third row in the table).

<img src="figures/Cyclic-ijk.svg"/>

\ifsolutions\else
\newpage
\fi

## Example

In the following diagram, a positive charge $q$ moves with a velocity in a region of space with a magnetic field.

<img src="figures/Lorentz_Force.svg"/>

For case f. in the figure above,

1. Write a vector equation for both $\bfvec{v}$ and $\bfvec{B}$ and use it to compute the force vector using $\bfvec{F} = q\bfvec{v}\times\bfvec{B}$ assuming that $\bfvec{B}=B_o\ihat$ and $|\bfvec{v}|=v_o$. Then compute the magnitude of $\bfvec{F}$.
2. Use $F = |q|vB\sin\phi$ to compute the magnitude of the force and use the right-hand rule to determine its direction. 

**Answer**

**f.1**

  $\bfvec{v}=-v_o\khat$, so $\bfvec{F} = q(-v_o\khat)\times (B_o\ihat)=-qv_oB_o(\khat\times \ihat)=-qv_oB_o\jhat$;

  $|\bfvec{F}|=|-qv_oB_o\jhat| = |-qv_oB_o||\jhat|=|q|v_oB_o$.

**f.2**

   $\phi=90^{\circ}$, so $F = |q|v_oB_o\sin(90^{\circ})=|q|v_oB_o$.

  The right--hand rule gives direction as $-\jhat$.

## Problem

Answer questions 1. and 2. given in the previous problem for cases a.--e. in the figure above. Assume that the magnitude of the velocity is $v_o$ and the magnitude of the magnetic field is $B_o$.

{\bf a.1}
\ifsolutions
$\bfvec{v}=v_o\jhat$, so $\bfvec{F} = q\,(v_o\jhat)\times (B_o\ihat)=qv_oB_o(\jhat\times \ihat)=-qv_oB_o\khat$; $|\bfvec{F}|=qv_oB_o$
\else
<div style="height:4em"/>
\fi

{\bf a.2}
\ifsolutions
$\phi=90^{\circ}$, so $F = qv_oB_o\sin(90^{\circ})=qv_oB_o$.
\fi

\ifsolutions\else
\newpage
\fi

\ifsolutions\else
<img src="figures/Lorentz_Force.svg"/>

The figure above is a copy of that on previous page.
\fi

{\bf b.1}
\ifsolutions
$\bfvec{v}=-v_o\jhat$, so $\bfvec{F} = -q\,(v_o\jhat)\times (B_o\ihat)=qv_oB_o(\jhat\times \ihat)=qv_oB_o\khat$; $|\bfvec{F}|=qv_oB_o$
\else
<div style="height:4em"/>
\fi
{\bf b.2}
\ifsolutions
$\phi=90^{\circ}$, so $F = qv_oB_o\sin(90^{\circ})=qv_oB_o$.
\else
<div style="height:4em"/>
\fi

{\bf c.1}
\ifsolutions
$\bfvec{v}=-v_o\ihat$, so $\bfvec{F} = -q(v_o\ihat)\times (B_o\ihat)=-qv_oB_o(\jhat\times \ihat)=0$; $|\bfvec{F}|=0$
\else
<div style="height:4em"/>
\fi

{\bf c.2}
\ifsolutions
$\phi=90^{\circ}$, so $F = qv_oB_o\sin(180^{\circ})=0$.
\else
<div style="height:4em"/>
\fi

{\bf d.1}
\ifsolutions
$\bfvec{v}=v_o\ihat$, so $\bfvec{F} = q(v_o\ihat)\times (B_o\ihat)=qv_oB_o(\ihat\times \ihat)=0$; $|\bfvec{F}|=0$
\else
<div style="height:4em"/>
\fi

{\bf d.2}
\ifsolutions
$\phi=90^{\circ}$, so $F = qv_oB_o\sin(0^{\circ})=0$.
\else
<div style="height:4em"/>
\fi

{\bf e.1}
\ifsolutions
$\bfvec{v}=v_o\khat$, so $\bfvec{F} = q\,(v_o\khat)\times (B_o\ihat)=qv_oB_o(\khat\times \ihat)=qv_oB_o\jhat$; $|\bfvec{F}|=qv_oB_o$
\else
<div style="height:4em"/>
\fi

{\bf e.2}
\ifsolutions
$\phi=90^{\circ}$, so $F = qv_oB_o\sin(90^{\circ})=qv_oB_o$.
\else
\newpage
\fi

# Trajectories

If the magnetic force on a charge particle is not zero the direction of its velocity vector will change. Because the magnetic force depends on the velocity vector direction, the magnetic force vector will also change.

For a charged particle moving in a region of space with a constant magnetic field (both in magnitude and direction), there are three general trajectories:

1. If the velocity is parallel to the magnetic field lines, the trajectory is a straight line because no magnetic forces are acting on it.
2. If velocity is perpendicular to the magnetic field lines, the trajectory is spiral. The particle rotates in a circle in the same plane as the velocity vector and drifts parallel or antiparallel to the field lines.
3. The velocity has parallel and perpendicular components to the magnetic field line. In this case, the particle will move at a constant speed parallel or antiparallel to the field lines and in a circle around the field line. The trajectory is a spiral.

## Problem

Use the simulation at https://ophysics.com/em8.html to verify the above three statements. State the settings that you used to create the trajectory. Also, state how the settings affected the trajectory and in which way (for example, for case $a.$, "changing $m$ did not change the shape of the type or shape of the trajectory"). 

1.
\ifsolutions
\else<div style="height:10em"/>\fi

2.
\ifsolutions\else<div style="height:10em"/>\fi

3.

\ifsolutions\else
\newpage
\fi

## Problem

Consider the following cases and describe the trajectory of the particle in words in the table below (e.g., "circle in $x$--$y$ plane; ccw when viewed from a point on $+z$ axis" or "spiral with motion in $+z$ direction; ccw when viewed from a point on $+z$ axis"). You may use the simulation to check some of your answers. 

\ifsolutions

{\bf Answer:} I determine the direction of rotation by using a right-hand rule -- wrap fingers around $\mathbf{B}$, and the direction of motion of a $+$ charge is in the opposite direction of my fingers. You'll learn later that this rule tells you that the magnetic field created by the charge that rotates around the magnetic field is in the opposite direction of the magnetic field that caused it to rotate.

Another way of doing this is drawing the $\mathbf{B}$ and $\mathbf{v}$ vectors and determining the direction of force - the trajectory will be a circle with the rotation direction that is required to rotate the velocity vector towards the force vector.

For both cases, I draw an $x$, $y$, $z$ axis, and the vectors $\mathbf{B}$, $\mathbf{v}$, and $\mathbf{F}$.

a. $\mathbf{B} =  B_o\hat{\mathbf{x}}$  $\mathbf{v} = v_o\hat{\mathbf{x}}$: Trajectory is straight line along $\hat{\mathbf{x}}$ direction.

b. $\mathbf{B} =  B_o\hat{\mathbf{z}}$ $\mathbf{v} = v_o\hat{\mathbf{x}}$: Trajectory is cw circle in $x$--$y$ plane when viewed from point on $+z$ axis

c. $\mathbf{B} = -B_o\hat{\mathbf{y}}$ $\mathbf{v} = v_o\hat{\mathbf{z}}$: Trajectory is ccw circle in $x$--$z$ plane when viewed from point on $+y$ axis

d. $\mathbf{B} = B_o\hat{\mathbf{x}} $ $\mathbf{v} = v_o\hat{\mathbf{x}}+v_o\hat{\mathbf{y}}$: Trajectory is cw circle in $y$--$z$ plane when viewed from point on the $+x$ axis. Spiral growing in +x direction.

e. $\mathbf{B} = -B_o\hat{\mathbf{y}}$ $\mathbf{v} = v_o\hat{\mathbf{y}}+v_o\hat{\mathbf{z}}$: Trajectory is ccw circle in $x$--$y$ plane when viewed from point on $+y$ axis. Spiral growing in $+y$ direction.
\else
$$
\begin{align*}
a.\quad & \mathbf{B} =  B_o\hat{\mathbf{x}}&  \mathbf{v} &= v_o\hat{\mathbf{x}} & & \bf{Trajectory =} \\\\ \\
b.\quad & \mathbf{B} =  B_o\hat{\mathbf{z}} &  \mathbf{v} & = v_o\hat{\mathbf{x}}& &  \bf{Trajectory =} \\\\ \\
c.\quad  & \mathbf{B} = -B_o\hat{\mathbf{y}} & \mathbf{v} & = v_o\hat{\mathbf{z}}& & \bf{Trajectory =} \\\\ \\
d.\quad  & \mathbf{B} = B_o\hat{\mathbf{x}} & \mathbf{v} & = v_o\hat{\mathbf{x}}+v_o\hat{\mathbf{y}}& &\bf{Trajectory =}\\\\ \\
e.\quad  & \mathbf{B} = -B_o\hat{\mathbf{y}} & \mathbf{v} & = v_o\hat{\mathbf{y}}+v_o\hat{\mathbf{z}}& & \bf{Trajectory =} & 
\end{align*}
$$
\fi
