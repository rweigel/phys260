```mdextension
Title: Electric Field Activity
```

# Overview

This activity covers topics in [Section 21.3-4 of Young and Freedman 2015, 14th Edition](https://drive.google.com/file/d/1JS_pBuNEwXdz9IzpSBFPJffgVacZmqN7/view?usp=sharing_remove_).

**Electric Force**

Coulomb's Law in compact form is

$$\bfvec{F}_{1\mbox{ on } 2}=kq_1q_2\frac{\rhat}{r^2}$$

where $\rhat$ is the unit vector that points from the position of $q_1$ to $q_2$ and $r$ is the distance between $q_1$ and $q_2$.

**Electric Field**

The electric field vector, $\bfvec{E}$, is a quantity that we assign to a point in space. Given this quantity, we can compute the force on a charge $Q$ will experience if it is placed at that point in space using the equation $\bfvec{F}=Q\bfvec{E}$.

To find $\bfvec{E}$ at any point in space, 
compute the force $\bfvec{F}$ due to all other charges on a hypothetical (or "test") charge $q_o$ at a point where you want to know $\bfvec{E}$. To find $\bfvec{E}$ at that point, divide $\bfvec{F}$ by $q_o$.

$$\bfvec{E} = \frac{\bfvec{F}}{q_o}$$

%To find $\bfvec{F}$ when a different charge $Q$ is placed where $q$ was, multiply $\bfvec{E}$ by $Q$.

# Example

Charge $q_1$ is at $(x,y)=(-a,-a)$.

Find the electric field at $(x,y)=(a,a)$ in the form $\bfvec{E}=E_x\ihat + E_y\jhat$.

**Solution**

To find the electric field at a point in space, we put a hypothetical "test" charge $q_o$ at that point, compute the force on it due to all other charges, and then use

$$\bfvec{E} = \frac{\bfvec{F}}{q_o}$$

The force a charge $q_1$ at $(x,y)=(-a,-a)$ exerts on a charge $q_2$ at $(x,y)=(a,a)$ was computed in a previous activity. We can use the answer after the replacement of $q_2$ with $q_o$. The result is

$\bfvec{F}=k\frac{q_1q_o}{8a^2}\left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right]$. The electric field is then $\bfvec{E} = \frac{\bfvec{F}}{q_o} = k\frac{q_1}{8a^2}\left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right]$

\newpage

# Problem

In the previous example, there was only one charge responsible for creating the electric field $\bfvec{E}$. To find the electric field when there are more charges, superposition can be used.

Charge $q_1 = +q$ is at $(x, y) = (a, 0)$, charge $q_2 = +q$ is at $(x, y) = (-a, 0)$, and charge $q_3 = -q$ is at $(x, y) = (0, a)$. Assume that the quantity associated with $q$ is positive. 

1. Draw this charge configuration below.

<div style="height:4em"/>

2. Why does it not make sense to ask what the electric force is at the origin?

<div style="height:2em"/>

In the following, 

3. Find the electric field at the origin due to $q_1$. Write your answer in the form $\bfvec{E}\_1=E_{x1}\ihat + E_{y1}\jhat$.

<div style="height:4em"/>

4. Find the electric field at the origin due to $q_2$. Write your answer in the form $\bfvec{E}\_2=E_{x2}\ihat + E_{y2}\jhat$.

<div style="height:4em"/>

5. Find the electric field at the origin due to $q_3$. Write your answer in the form $\bfvec{E}\_3=E_{x3}\ihat + E_{y3}\jhat$.

<div style="height:4em"/>

6. Find the electric field at the origin. Write your answer in the form $\bfvec{E}=E_{x}\ihat + E_{y}\jhat$.

<div style="height:4em"/>

7. Will your answers to 3.-6. change if the problem had asked for the electric field at a different position? If so, which answers?

\newpage

8. Find the electric field at the origin if charge $q_1=2q$ (instead of $q$).

<div style="height:10em"/>

9. Find the electric field at the origin if charge $q_1=-2q$ (instead of $q$).