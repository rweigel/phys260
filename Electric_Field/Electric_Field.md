```mdextension
Title: Electric Field and $\rhat$
```

# Overview

This activity covers topics in [Section 21.4 of Young and Freedman 2015, 14th Edition](https://drive.google.com/file/d/1JS_pBuNEwXdz9IzpSBFPJffgVacZmqN7/view?usp=sharing_remove_).

The electric field vector, $\bfvec{E}$, is a quantity that we assign to a point in space. Given this quantity, we can compute the force on a charge $Q$ will experience if it is placed at that point in space using the equation $\bfvec{F}=Q\bfvec{E}$. The direction of $\mathbf{E}$ is also the direction a charge will begin to move if released from rest.

To find $\bfvec{E}$ at any point in space, 
compute the force $\bfvec{F}$ due to all other charges on a hypothetical (or "test") charge $q_o$ at a point where you want to know $\bfvec{E}$. To find $\bfvec{E}$ at that point, divide $\bfvec{F}$ by $q_o$.

$$\bfvec{E} = \frac{\bfvec{F}}{q_o}$$

%To find $\bfvec{F}$ when a different charge $Q$ is placed where $q$ was, multiply $\bfvec{E}$ by $Q$.

# Example

Charge $q_1$ is at $(x,y)=(-a,-a)$. Find the electric field at $(x,y)=(a,a)$ in the form $\bfvec{E}=E_x\ihat + E_y\jhat$. Also find $E$. (Note that $E$ and $|\mathbf{E}|$ are used interchangebly.)

**Solution**

To find the electric field at a point in space, we put a hypothetical "test" charge $q_o$ at that point, compute the force on it due to all other charges, and then use

$$\bfvec{E} = \frac{\bfvec{F}}{q_o}$$

The force a charge $q_1$ at $(x,y)=(-a,-a)$ exerts on a charge $q_2$ at $(x,y)=(a,a)$ was computed in a previous activity. We can use that answer after the replacement of $q_2$ with $q_o$. The result is

$$\bfvec{F}_{q_1\text{ on } q_o}=k\frac{|q_1q_o|}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat)$$

We also found that we got the same result if $q_1$ and $q_o$ are are positive or both are negative. If $q_1$ was positive and $q_o$ is negative, or vice-versa, we found the sign changed:

$$\bfvec{F}_{q_1\text{ on } q_o}=-k\frac{|q_1q_o|}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat)$$

Based on this, we can write a single equation for all possibilities:

$$\bfvec{F}_{q_1\text{ on } q_o}=k\frac{q_1q_o}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat)$$

The electric field at the location of $q_o$ is then 

$\ds\bfvec{E}_{\text{at }(a,a) \text{ due to }q_1} = \frac{\bfvec{F}}{q_o} = k\frac{q_1}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat) =k\frac{q_1}{8a^2}\left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right]$

where the fact that $\sin 45^\circ=\cos 45^\circ=1/\sqrt{2}$ was used.

Sign check: It is easy to make a sign error when computing electric fields and forces. The electric field at points in the direction a positve charge will move if released from rest. Suppose $q_1$ is positive. Our equation predicts that a charge will move up and to the right. Suppose $q_1$ is negative. Our equation predicts that a charge will move down and to the left.

# Problem I

Charge $q_1$ is at $(x,y)=(-a,a)$. At $(x,y)=(a, 0)$, find $\mathbf{E}$ in the form $\bfvec{E}=E_x\ihat + E_y\jhat$ and $E$.

<img src="../Electric_Force/figures/grid.svg" style="width:100%"/>

\newpage

# Unit Vector

Previously, when computing the electric force between two charges, you used the formula $F=k{|q_1q_2|}/{r^2}$ to find the magnitude of the force and then used a diagram to write $\mathbf{F}$ in the form $\bfvec{F}=F_x\ihat + F_y\jhat$. A similar process was used for computing $\bfvec{E}$ above (because we computed $\mathbf{F}$ as part of the process). The textbook provides an equation for the electric field that requires a slightly different method of calculation.

The equation for the electric field using a unit vector is

$$\bfvec{E}_{\text{due to }q_1}=kq_1\frac{\rhat}{r^2}$$

where $\rhat$ is the unit vector that points from the position of $q_1$ to the point in space where we want to know $\mathbf{E}$ and $r$ is the distance between $q_1$ and that point.

To find $\rhat$, 

1. draw a vector, $\mathbf{r}$ from $q_1$ to the point in space where you want to know $\mathbf{E}$;
2. Write $\mathbf{r}$ in the form $\mathbf{r}=r_x\ihat+r_y\yhat$; then
3. $\rhat=\mathbf{r}/r$, where $r=\sqrt{r_x^2+r_y^2}$.

## Example

If $q_1$ is at $(x,y)=(-a,-a)$, find the electric field using $\bfvec{E}_{\text{due to }q_1}=kq_1{\rhat}/{r^2}$ at $(x,y)=(a,a)$.

**Solution**

The calculation of $\rhat$ is shown in the following diagram.

<img src="figures/Two_Charges.svg" style="width:100%"/>

Substitution gives

$$\bfvec{E}_{\text{at }(a,a)\text{ due to }q_1}=kq_1\frac{\rhat}{r^2} = k\frac{q_1}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat) =k\frac{q_1}{8a^2}\left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right]$$

which is the same result obtained in the previous example, as expected.

Note that we did not need to compute the magnitude of the electric field, $E$, to compute $\mathbf{E}$. It can be computed from the above equation using

$$|\mathbf{E}|=E=\sqrt{E_x^2+E_y^2}$$

One can plug in $E_x=k\frac{q_1}{8a^2}\cos 45^\circ$ and $E_y=k\frac{q_1}{8a^2}\sin 45^\circ$ and use the identities $\sqrt{c^2}=|c|$ (where $c$ is a real number) and $\sin^2\theta + \cos^2\theta=1$ to show that $E=k|q_1|/{8a^2}$. There is an easier way. Taking the magnitude of both sides of

$\ds\bfvec{E}=kq_1\frac{\rhat}{r^2}\quad$
gives
$\quad\ds|\bfvec{E}|=k|q_1|\frac{|\rhat|}{r^2}$.

The magnitude of a unit vector is $1$ (hence the name), so

$\ds|\bfvec{E}|=k|q_1|\frac{1}{r^2}=\frac{k|q_1|}{8a^2},\thickspace$ as before.

\newpage

# Problem II

Charge $q_1$ is at $(x,y)=(-a,a)$. Find the electric field at $(x,y)=(a, 0)$ using $\bfvec{E}_{\text{at }(a,0)\text{ due to }q_1}=kq_1{\rhat}/{r^2}$ at $(x,y)=(a,a)$.

<img src="../Electric_Force/figures/grid.svg" style="width:100%"/>

\newpage

# Problem III - Superposition

In the previous examples, only one charge was responsible for creating the electric field $\bfvec{E}$. When there are more charges, superposition can be used.

Charge $q_1 = +q$ is at $(x, y) = (a, 0)$, charge $q_2 = +q$ is at $(x, y) = (-a, 0)$, and charge $q_3 = -q$ is at $(x, y) = (0, a)$. Assume that $q$ is a positive number.

1. Draw this charge configuration below.

<img src="../Electric_Force/figures/grid.svg" style="width:100%"/>

2. Why does it not make sense to ask what the electric force is at the origin?

<div style="height:2em"/>

In the following, 

3. Find the electric field at the origin due to $q_1$. Write your answer in the form $\bfvec{E}\_1=E_{x1}\ihat + E_{y1}\jhat$.

<div style="height:6em"/>

4. Find the electric field at the origin due to $q_2$. Write your answer in the form $\bfvec{E}\_2=E_{x2}\ihat + E_{y2}\jhat$.

<div style="height:6em"/>

5. Find the electric field at the origin due to $q_3$. Write your answer in the form $\bfvec{E}\_3=E_{x3}\ihat + E_{y3}\jhat$.

<div style="height:6em"/>

6. Find the electric field at the origin. Write your answer in the form $\bfvec{E}=E_{x}\ihat + E_{y}\jhat$.

<div style="height:6em"/>

7. Will your answers to 3.-6. change if the problem had asked for the electric field at a different position? If so, which answers?

<div style="height:6em"/>

8. Find the electric field at the origin if charge $q_1=2q$ (instead of $q$).

<div style="height:12em"/>

9. Find the electric field at the origin if charge $q_1=-2q$ (instead of $q$).