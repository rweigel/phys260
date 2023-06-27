```mdextension
Title: Electric Field
```

# Overview

The electric field vector, $\bfvec{E}$, is a quantity assigned to a point in space. Given this quantity, we can compute the force on a charge $Q$ will experience if it is placed at that point using the equation $\bfvec{F}=Q\bfvec{E}$. The direction of $\bfvec{E}$ is also the direction a charge will begin to move if released from rest.

To find $\bfvec{E}$ at any point in space, 
compute the force $\bfvec{F}$ due to all other charges on a hypothetical (or "test") charge $q_o$ at a point where you want to know $\bfvec{E}$. To find $\bfvec{E}$ at that point, divide $\bfvec{F}$ by $q_o$.

$$\bfvec{E} = \frac{\bfvec{F}}{q_o}$$

%To find $\bfvec{F}$ when a different charge $Q$ is placed where $q$ was, multiply $\bfvec{E}$ by $Q$.

# Example I

Charge $q_1$ is at $(x,y)=(-a,-a)$. Find the electric field at $(x,y)=(a,a)$ in the form $\bfvec{E}=E_x\ihat + E_y\jhat$. Also, find $E$. (Note that $E$ and $|\bfvec{E}|$ are used interchangebly.)

**Solution**

To find the electric field at a point in space, we put a hypothetical "test" charge $q_o$ at that point, compute the force on it due to all other charges, and then use

$$\bfvec{E} = \frac{\bfvec{F}}{q_o}$$

The force a positive charge $q_1$ at $(x,y)=(-a,-a)$ exerts on a positive charge $q_2$ at $(x,y)=(a, a)$ was computed in a previous activity.

$$\bfvec{F}_{q_1\text{ on } q_2}=k\frac{|q_1q_2|}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat)$$

We also found that this equation applies when $q_1$ and $q_2$ are both positive or both are negative. If $q_1$ was positive and $q_2$ was negative, or vice-versa, we found the sign changed:

$$\bfvec{F}_{q_1\text{ on } q_2}=-k\frac{|q_1q_2|}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat)$$

Based on this, we can write a single equation for all possibilities:

$$\bfvec{F}_{q_1\text{ on } q_2}=k\frac{q_1q_2}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat)$$

If we replace $q_2$ with $q_o$, this is

$$\bfvec{F}_{q_1\text{ on } q_o}=k\frac{q_1q_o}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat)$$

The electric field at the location of $q_o$ is then 

$\ds\bfvec{E}_{\text{at }(a,a) \text{ due to }q_1} = \frac{\bfvec{F}}{q_o} = \frac{kq_1}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat) =\frac{kq_1}{8a^2}\left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right]$,

where the fact that $\sin 45^\circ=\cos 45^\circ=1/\sqrt{2}$ was used. The magnitude is $E=\sqrt{E_x^2+E_y^2}=k|q_1|/8a^2$.

Sign check: When computing electric fields and forces, it is easy to make a sign error. The electric field vector points in the direction a positive charge will move if released there from rest. Suppose $q_1$ is positive. Our equation predicts that a positive charge released from rest at $(a, a)$ will move up and to the right. Suppose $q_1$ is negative. Our equation predicts that a positive charge will move down and to the left. This is consistent with the fact that like charges repel and unlike charges attract.

# Problem I

Charge $q_1$ is at $(x,y)=(-a,a)$. At $(x,y)=(a, 0)$, find $\bfvec{E}$ in the form $\bfvec{E}=E_x\ihat + E_y\jhat$. Check signs of the components of $\bfvec{E}$ using the technique used in Example I. Also, find $E$.

<img src="../Electric_Force/figures/grid.svg" style="width:100%"/>

\ifsolutions
{\bf Answer}:

From Problem II on the Electric Force Activity, if $q_2$ is at $(x,y)=(a, 0)$ (and using the arguments in the previous example to drop the absolute value sign),

$$\bfvec{F}_{q_1\text{ on } q_2}=k\frac{q_1q_2}{5a^2}\left(\frac{2}{\sqrt{5}}\ihat -\frac{2}{\sqrt{5}}\jhat\right)$$

Replacing $q_2$ with a test charge $q_o$,

$$\bfvec{F}_{q_1\text{ on } q_o}=k\frac{q_1q_o}{5a^2}\left(\frac{2}{\sqrt{5}}\ihat -\frac{2}{\sqrt{5}}\jhat\right)$$

$\ds\bfvec{E}_{\text{at }(a,0) \text{ due to }q_1} = \frac{\bfvec{F}}{q_o}=\frac{kq_1}{5a^2}\left(\frac{2}{\sqrt{5}}\ihat -\frac{2}{\sqrt{5}}\jhat\right)$

\fi

\newpage

# Problem II

Charge $q_1$ is at $(x,y)=(-a,a)$. Find the electric field at $(x,y)=(a, 0)$, find $\bfvec{E}$ in the form $\bfvec{E}=E_x\ihat + E_y\jhat$. Check signs of the components of $\bfvec{E}$ using the technique used in Example I. Also, find $E$.

<img src="../Electric_Force/figures/grid.svg" style="width:100%"/>

\ifsolutions
{\bf Answer}:

$\ds\bfvec{E}_{\text{at }(a,0) \text{ due to }q_1}=\frac{kq_1}{5a^2}\left(\frac{2}{\sqrt{5}}\ihat -\frac{2}{\sqrt{5}}\jhat\right)$, which matches the solution to Problem I, as expected.

\fi
