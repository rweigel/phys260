```mdextension
Title: The $\rhat$ Unit Vector
```

% Figures:
% https://www.mathcha.io/editor/M55KMuQLiLmH9Vgp0Ptw6QGB3HnpzJnnuM6VoB7

# The $\rhat$ Unit Vector

Previously, when computing the electric force between two charges, you used the formula $E=k{|q|}/{r^2}$ to find the electric field and then used a diagram to write $\bfvec{E}$ in the form $\bfvec{E}=E_x\ihat + E_y\jhat$.

An alternative, and more direct, approach is to use an equation for electric field using a unit vector $\rhat$:

$$\bfvec{E}_{\text{due to }q}=kq\frac{\rhat}{r^2}\thinspace,$$

where $\rhat$ is the unit vector that points from the position of $q_1$ to the point in space where we want to know $\bfvec{E}$, and $r$ is the distance between $q_1$ and that point. Note that in this equation, we use $q$ and not $|q|$.

To find $\rhat$, 

1. draw a vector, $\bfvec{r}$ from $q_1$ to the point in space where you want to know $\bfvec{E}$;
2. Write $\bfvec{r}$ in the form $\bfvec{r}=r_x\ihat+r_y\jhat$; then
3. $\rhat=\bfvec{r}/r$, where $r=\sqrt{r_x^2+r_y^2}$.

# Example

If $q_1$ is at $(x,y)=(-a,-a)$, find the electric field at $(x,y)=(a,a)$ using $\bfvec{E}_{\text{due to }q_1}=kq_1{\rhat}/{r^2}$. Also, find $E$.

**Solution**

The calculation of $\rhat$ is shown in the following diagram.

<img src="figures/Two_Charges.svg" style="width:100%"/>

Substitution gives

$$\bfvec{E}_{\text{at }(a,a)\text{ due to }q_1}=kq_1\frac{1}{r^2}\rhat = kq_1\frac{1}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat) =\frac{kq_1}{8a^2}\left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right]\thinspace,$$

which is the same result obtained in the previous example, as expected.

To calculate $|\bfvec{E}|$, we can use

$$|\bfvec{E}|=E=\sqrt{E_x^2+E_y^2}$$

and plug in $E_x=k\frac{q_1}{8a^2}\frac{1}{\sqrt{2}}$ and $E_y=k\frac{q_1}{8a^2}\frac{1}{\sqrt{2}}$ and use $\sqrt{c^2}=|c|$ (where $c$ is a real number) to show that $E=k|q_1|/{8a^2}$. There is an easier way. Taking the magnitude of both sides of

$\ds\bfvec{E}=kq_1\frac{\rhat}{r^2}\quad$
gives
$\quad\ds|\bfvec{E}|=k|q_1|\frac{|\rhat|}{r^2}$.

The magnitude of a unit vector is $1$, so

$\ds|\bfvec{E}|=k|q_1|\frac{1}{r^2}=\frac{k|q_1|}{8a^2},\thickspace$ as before.

# Problem

Charge $q_1$ is at $(x,y)=(-a,a)$. Find the electric field at $(x,y)=(a, 0)$ using $\bfvec{E}_{\text{at }(a,0)\text{ due to }q_1}=kq_1{\rhat}/{r^2}$. Check signs of the components of $\bfvec{E}$ using the technique used in the Example. Also, find $|\bfvec{E}|$.

<img src="../Electric_Force/figures/grid.svg" style="width:100%"/>

\ifsolutions
{\bf Answer}:

$\bfvec{r}=2a\ihat-a\jhat$,
$\quad$
$\ds\rhat=\frac{2}{\sqrt{5}}\ihat-\frac{1}{\sqrt{5}}\jhat$,
$\quad$ $r^2=5a^2$

$\ds\bfvec{E}_{\text{at }(a,0) \text{ due to }q_1}=\frac{kq_1}{5a^2}\left(\frac{2}{\sqrt{5}}\ihat -\frac{2}{\sqrt{5}}\jhat\right)$, which matches the solution to Problem I, as expected.

\fi

# Question

Can you solve an Electric Force (Coulomb's Law) problem using $\rhat$ notation? If yes, what is the equation for the electric force using $\rhat$?