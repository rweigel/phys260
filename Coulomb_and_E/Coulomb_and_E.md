# Overview

See also [Chapter 21 of Young and Freedman 2015, 14th Edition](https://drive.google.com/file/d/1JS_pBuNEwXdz9IzpSBFPJffgVacZmqN7/view?usp=sharing_remove_)

**Electric Force**

*Magnitude*: $\displaystyle F=\frac{1}{4\pi\epsilon_o}\frac{|q_1q_2|}{r^2}$

*Direction*: Force is along line that connects $q_1$ and $q_2$. Direction depends on signs of $q_1$ and $q_2$. (Likes repel, opposites attract.) $r$ is separation distance. Sometimes $k$ is used in place of the proportionality constanat $1/4\pi\epsilon_o$.

**Electric Field**

Compute force $\mathbf{F}$ due to all other charges on a hypothetical charge $q$ at point where you want to compute $\mathbf{E}$. To find $\mathbf{E}$ at that point, divide $\mathbf{F}$ by $q$.

$$\mathbf{E} = \frac{\mathbf{F}}{q}$$

To find $\mathbf{F}$ when a different charge $Q$ is placed where $q$ was, multiply $\mathbf{E}$ by $Q$.

\newpage

# Problem

Charge $q_1$ is at $(x, y) = (a, a)$.

1. Find the magnitude of the electric field at $(x, y) = (a, 2a)$. Show your work. Compare your answer with other students in your group.

<div style="height:4em"/>

2. Find the direction of the electric field at $(x, y) = (a, 2a)$ if $q_1$ is positive. Express your answer as an angle with respect to the $x$-axis, with counterclockwise rotation being positive. Show your work.

<div style="height:4em"/>

3. If there are no other charges besides $q_1$, why it does not make sense to ask what the electric force is at $(x, y) = (a, 2a)$?

<div style="height:4em"/>

4. If a charge $Q$ is placed at $(a, 2a)$, what will be the magnitude of the electric force that is exerted on it? Will the direction of this force depend on the signs of $q_1$ and $Q$?

\newpage

# $\mathbf{E}$ for a System of Charges

Charge $q_1 = +q$ is at $(x, y) = (a, 0)$, charge $q_2 = +q$ is at $(x, y) = (-a, 0)$, and charge $q_3 = -q$ is at $(x, y) = (0, a)$. Assume that the quantity associated with $q$ is positive. Draw this charge configuration on the provided graph paper.

<img src="figures/grid-w100pct-w20pps-h200px-h20pps.svg" style="width:100%"/>

1. Find the electric field magnitude and direction at the origin. Show your work in the space below.

<div style="height:8em"/>

2. Find the electric field magnitude and direction at the origin if $q_1=-q$.

<div style="height:8em"/>

3. What is still confusing about electric forces and fields? If nothing, what is one thing that you learned from this tutorial?

# Overview

This activity covers topics  in [Section 21.3-4 of Young and Freedman 2015, 14th Edition](https://drive.google.com/file/d/1JS_pBuNEwXdz9IzpSBFPJffgVacZmqN7/view?usp=sharing_remove_).

**Electric Force**

Coulomb's Law in compact form is

$$\mathbf{F}_{1\mbox{ on } 2}=kq_1q_2\frac{\hat{\mathbf{r}}}{r^2}$$

**Electric Field**

The electric field vector, $\mathbf{E}$ is a quantity that we assign to a point in space. Given this quantity, we can compute the force on a charge $Q$ will experience if it is placed at that point in space using the equation $\mathbf{F}=Q\mathbf{E}$.

To find $\mathbf{E}$ at any point in space, 
compute the force $\mathbf{F}$ due to all other charges on a hypothetical (or "test") charge $q_o$ at point where you want to know $\mathbf{E}$. To find $\mathbf{E}$ at that point, divide $\mathbf{F}$ by $q_o$.

$$\mathbf{E} = \frac{\mathbf{F}}{q_o}$$

%To find $\mathbf{F}$ when a different charge $Q$ is placed where $q$ was, multiply $\mathbf{E}$ by $Q$.

\newpage

# Example

Charge $q_1$ is at $(x,y)=(-a,-a)$.

Find the electric field at $(x,y)=(a,a)$ in the form $\mathbf{E}=E_x\xhat + E_y\yhat$.

**Solution**

According to the perscription given, to find the electric field at a point in space, we put a hypothetical "test" charge $q_o$ at that point, compute the force on it due to all other charges, and then use

$$\mathbf{E} = \frac{\mathbf{F}}{q_o}$$

The force a charge $q_1$ at $(x,y)=(-a,-a)$ exerts on a charge $q_2$ at $(x,y)=(a,a)$ was computed previously. We can use the answer after replacement of $q_2$ with $q_o$. This gives

$$\mathbf{F}=k\frac{q_1q_o}{8a^2}\left[\frac{1}{\sqrt{2}}\xhat + \frac{1}{\sqrt{2}}\yhat\right]$$

The electric field is then

$$\mathbf{E} = \frac{\mathbf{F}}{q_o} = k\frac{q_1}{8a^2}\left[\frac{1}{\sqrt{2}}\xhat + \frac{1}{\sqrt{2}}\yhat\right]$$

# Problem

In the previous example, there was only one charge responsible for creating the electric field $\mathbf{E}$. To find the electric field when there are more charges, superposition can be used.

Charge $q_1 = +q$ is at $(x, y) = (a, 0)$, charge $q_2 = +q$ is at $(x, y) = (-a, 0)$, and charge $q_3 = -q$ is at $(x, y) = (0, a)$. Assume that the quantity associated with $q$ is positive. 

1. Draw this charge configuration on the provided graph paper.

<img src="figures/grid-w100pct-w20pps-h200px-h20pps.svg" style="width:100%"/>

In the following, 

2. Find the electric field at the origin due to $q_1$. Write your answer in the form $\mathbf{E}\_1=E_{x1}\xhat + E_{y1}\yhat$.


3. Find the electric field at the origin due to $q_2$. Write your answer in the form $\mathbf{E}\_2=E_{x2}\xhat + E_{y2}\yhat$.


4. Find the electric field at the origin due to $q_3$. Write your answer in the form $\mathbf{E}\_3=E_{x3}\xhat + E_{y3}\yhat$.


5. Find the electric field at the origin. Write your answer in the form $\mathbf{E}=E_{x}\xhat + E_{y}\yhat$.


6. Will your answers to 2.-5. change if the problem had asked for the electric field at a different position? If so, which answers?


7. Find the electric field at the origin if charge $q_1=2q$ (instead of $q$).