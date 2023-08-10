```mdextension
Title: The $\rhat$ Unit Vector
```

% Figures:
% https://www.mathcha.io/editor/M55KMuQLiLmH9Vgp0Ptw6QGB3HnpzJnnuM6VoB7

# The $\rhat$ Unit Vector

One approach to finding the electric force between two charges is to use
$F=k{|q_1q_2|}/{r^2}$ to find the magnitude and a diagram to write $\bfvec{F}$ in the form $\bfvec{F}=F_x\ihat + F_y\jhat$.

An alternative, and more direct, approach is to use an equation for electric force using a unit vector $\rhat$:

$$\bfvec{F}_{q_1\text{ on }q_2}=kq_1q_2\frac{\rhat}{r^2}$$

where $\rhat$ is the unit vector that points from the position of $q_1$ to the position of $q_2$, and $r$ is the distance between $q_1$ and $q_2$.

To find $\rhat$, 

1. draw a vector, $\bfvec{r}$, from $q_1$ to $q_2$;
2. Write $\bfvec{r}$ in the form $\bfvec{r}=r_x\ihat+r_y\jhat$; then
3. $\rhat=\bfvec{r}/r$, where $r=\sqrt{r_x^2+r_y^2}$.

Similarly, the equation for electric field using a unit vector $\rhat$ is

$$\bfvec{E}_{\text{due to }q}=kq\frac{\rhat}{r^2}$$

where $\rhat$ is the unit vector that points from the position of $q_1$ to the point in space where we want to know $\bfvec{E}$, and $r$ is the distance between $q_1$ and that point. 

To find $\rhat$, 

1. draw a vector, $\bfvec{r}$ from $q_1$ to the point in space where you want to know $\bfvec{E}$;
2. Write $\bfvec{r}$ in the form $\bfvec{r}=r_x\ihat+r_y\jhat$; then
3. $\rhat=\bfvec{r}/r$, where $r=\sqrt{r_x^2+r_y^2}$.

Note that in the equations for $\bfvec{F}$ and $\bfvec{E}$, we do not need to take the absolute value of the charges.

# Example I

Charge $q_1$ is at $(x,y)=(-a,-a)$ and charge $q_2$ is at $(a, a)$. Find

1. $\rhat$
2. $\bfvec{F}_{q_1\text{ on }q_2}$
3. $F_{q_1\text{ on }q_2}$

**Solution**

The calculation of $\rhat$ is shown in the following diagram.

<img src="figures/Two_Charges.svg" style="width:100%"/>

Substitution gives

$$\bfvec{F}_{q_1\text{ on }q_2}=kq_1q_2\frac{\rhat}{r^2} = \frac{kq_1q_2}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat) =\frac{kq_1q_2}{8a^2}\left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right]$$

Check: if $q_1$ and $q_2$ are both positive, the force on $q_2$ is upwards and to the right, as expected.

# Problem I

Charge $q_1$ is at $(x,y)=(-a,a)$ and charge $q_2$ is at $(a, 0)$. Find

1. $\rhat$
2. $\bfvec{F}_{q_1\text{ on }q_2}$
3. $F_{q_1\text{ on }q_2}$

# Example II

If $q_1$ is at $(x,y)=(-a,-a)$, find 

1. $\rhat$
2. $\bfvec{E}_{\text{at }(a,a)\text{ due to }q_1}$
3. $E_{\text{at }(a,a)\text{ due to }q_1}$

**Solution**

The calculation of $\rhat$ is shown in the following diagram.

<img src="figures/Two_Charges.svg" style="width:100%"/>

Substitution gives

$$\bfvec{E}_{\text{at }(a,a)\text{ due to }q_1}=kq_1\frac{\rhat}{r^2} = kq_1\frac{1}{8a^2}(\cos 45^\circ \ihat + \sin 45^\circ \jhat) =\frac{kq_1}{8a^2}\left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right]$$

Check: If a positive charge was placed at $(x,y)=(a,a)$, it would tend to move up and to the right, which is consitent with the signs on the components of the electric field found above.

To calculate $|\bfvec{E}|$, we can use

$$|\bfvec{E}|=E=\sqrt{E_x^2+E_y^2}$$

and plug in $E_x=k\frac{q_1}{8a^2}\frac{1}{\sqrt{2}}$ and $E_y=k\frac{q_1}{8a^2}\frac{1}{\sqrt{2}}$ and use $\sqrt{c^2}=|c|$ (where $c$ is a real number) to show that $E=k|q_1|/{8a^2}$. There is an easier way. Taking the magnitude of both sides of

$\ds\bfvec{E}=kq_1\frac{\rhat}{r^2}\quad$
gives
$\quad\ds|\bfvec{E}|=k|q_1|\frac{|\rhat|}{r^2}$.

The magnitude of a unit vector is $1$, so

$\ds|\bfvec{E}|=k|q_1|\frac{1}{r^2}=\frac{k|q_1|}{8a^2}$.

# Problem II

If $q_1$ is at $(x,y)=(-a,a)$, find 

1. $\rhat$
2. $\bfvec{E}_{\text{at }(a,0)\text{ due to }q_1}$
3. $E_{\text{at }(a,0)\text{ due to }q_1}$

<img src="../Electric_Force/figures/grid.svg" style="width:100%"/>

\ifsolutions
{\bf Answer}:

$\bfvec{r}=2a\ihat-a\jhat$,
$\quad$ $r=\sqrt{5}a$
$\quad$
$\ds\rhat=\frac{2}{\sqrt{5}}\ihat-\frac{1}{\sqrt{5}}\jhat$,


$\ds\bfvec{E}_{\text{at }(a,0) \text{ due to }q_1}=\frac{kq_1}{5a^2}\left(\frac{2}{\sqrt{5}}\ihat -\frac{2}{\sqrt{5}}\jhat\right)$.

\fi
