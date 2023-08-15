```mdextension
Title: Electric Field
```

% Figures:
% https://www.mathcha.io/editor/M55KMuQLiLmH9Vgp0Ptw6QGB3HnpzJnnuM6VoB7

# Overview

The electric field vector, $\bfvec{E}$, is a quantity assigned to a point in space. Given this quantity, we can compute the force on a charge $Q$ will experience if it is placed at that point using the equation $\bfvec{F}=Q\bfvec{E}$. The direction of $\bfvec{E}$ is also the direction a charge will begin to move if released from rest.

To find $\bfvec{E}$ at any point in space, 
compute the force $\bfvec{F}$ due to all other charges on a hypothetical (or "test") charge $q_o$ that has an infinitesimal charge and size at a point where you want to know $\bfvec{E}$. To find $\bfvec{E}$ at that point, divide $\bfvec{F}$ by $q_o$.

$$\bfvec{E}_{\text{due to }q} = \frac{\bfvec{F}_{q\text{ on }q_o}}{q_o}$$

%To find $\bfvec{F}$ when a different charge $Q$ is placed where $q$ was, multiply $\bfvec{E}$ by $Q$.

# Example I

A positive charge $q_1$ is at $(x,y)=(-a,-a)$. Find the electric field at $(x,y)=(a,a)$ in the form $\bfvec{E}=E_x\ihat + E_y\jhat$. Also, find $E$. (Note that $E$ and $|\bfvec{E}|$ are used interchangeably.)

**Solution**

To find the electric field at a point in space, we put a hypothetical and positive "test" charge $q_o$ at that point, compute the force on it due to all other charges, and then use

$$\bfvec{E} = \frac{\bfvec{F}}{q_o}$$

The force a positive charge $q_1$ at $(x,y)=(-a,-a)$ exerts on a positive charge $q_2$ at $(x,y)=(a, a)$ was computed in a previous activity. The result was

$$\bfvec{F}_{q_1\text{ on } q_2}=k\frac{|q_1q_2|}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat)$$

Because both charges are positive, we can drop the absolute value in the above equation, giving

$$\bfvec{F}_{q_1\text{ on } q_2}=k\frac{q_1q_2}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat)$$

If we replace $q_2$ with $q_o$, this is

$$\bfvec{F}_{q_1\text{ on } q_o}=k\frac{q_1q_o}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat)$$

The electric field at the location of $q_o$ is then 

$\ds\bfvec{E}_{\text{at }(a,a) \text{ due to }q_1} = \frac{\bfvec{F}}{q_o} = \frac{kq_1}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat) =\frac{kq_1}{8a^2}\left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right]$,

where the fact that $\sin 45^\circ=\cos 45^\circ=1/\sqrt{2}$ was used. The magnitude is $E=k|q_1|/8a^2$.

Sign check: When computing electric fields and forces, it is easy to make a sign error. The electric field vector points in the direction a positive charge will move if released there from rest. $q_1$ was given to be positive. Our equation predicts that a positive charge released from rest at $(a, a)$ will move up and to the right. Suppose $q_1$ is negative. Our equation predicts that a positive charge will move down and to the left. This is consistent with the fact that like charges repel and unlike charges attract. (Note that we only derived the equation for $\bfvec{E}$ when $q_1$ was positive, but it turns out that the equation we arrive at is correct when $q_1$ is negative.)

# Problem I

A positive charge $q_1$ is at $(x,y)=(-a,a)$. At $(x,y)=(a, 0)$, find $\bfvec{E}$ in the form $\bfvec{E}=E_x\ihat + E_y\jhat$. Check signs of the components of $\bfvec{E}$ using the technique used in Example I. Also, find $E$.

\ifsolutions
{\bf Answer}:

From Problem II on the Electric Force Activity, if $q_2$ is at $(x,y)=(a, 0)$ (and using the arguments in the previous example to drop the absolute value sign),

$$\bfvec{F}_{q_1\text{ on } q_2}=k\frac{q_1q_2}{5a^2}\left(\frac{2}{\sqrt{5}}\ihat -\frac{2}{\sqrt{5}}\jhat\right)$$

Replacing $q_2$ with a test charge $q_o$,

$$\bfvec{F}_{q_1\text{ on } q_o}=k\frac{q_1q_o}{5a^2}\left(\frac{2}{\sqrt{5}}\ihat -\frac{2}{\sqrt{5}}\jhat\right)$$

$\ds\bfvec{E}_{\text{at }(a,0) \text{ due to }q_1} = \frac{\bfvec{F}}{q_o}=\frac{kq_1}{5a^2}\left(\frac{2}{\sqrt{5}}\ihat -\frac{2}{\sqrt{5}}\jhat\right)$

$E = k|q_1|/5a^2$
\else
<img src="../Electric_Force/figures/grid.svg" style="width:100%"/>
\fi

\newpage

# Problem II

To find the electric field at a point in space in Example I and Problem I, we first computed the force on a charge at that point and then divided the result by the charge.

An alternative approach is to start with the equation for the magnitude of the elctric field due to a charge $q$ at a point that is a distance $r$ from the charge:

$E_{\text{due to }q}=k{|q|}/{r^2}$

Charge $q_1$ is at $(x,y)=(a, a)$. Find the magnitude of the electric field, $E$, at $(x,y)=(0, 0)$ using the above formula and then find $\bfvec{E}$ in the form $\bfvec{E}=E_x\ihat + E_y\jhat$.

\ifsolutions
{\bf Answer}:

$E = kq/2a^2$

$\ds\bfvec{E}_{\text{at }(0,0) \text{ due to }q_1}=-\frac{kq_1}{2a^2}\left(\frac{1}{\sqrt{2}}\ihat +\frac{1}{\sqrt{2}}\jhat\right)$

\else

<img src="../Electric_Force/figures/grid.svg" style="width:100%"/>

\fi
