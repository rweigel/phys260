```mdextension
Title: Computing $\mathbf{B}$
```

# Introduction

In previous activities, you computed the force on moving charges in a region of space where there is a magnetic field. No mention was made of how the magnetic field was created.

In this activity, you compute the magnetic field created by moving charges.

The magnetic field due to a point charge $q$ moving with velocity $\bfvec{v}$ (when $v$ is small compared to the speed of light) is

$$
\bfvec{B} = \frac{\mu_o}{4\pi}\frac{q\bfvec{v}\times\hat{\mathbf{r}}}{r^2}
$$

where $\rhat$ is the unit vector that points from the position of $q$ to the point in space where we want to know $\bfvec{B}$, and $r$ is the distance between $q$ and that point.

To find $\rhat$, 

1. draw a vector, $\bfvec{r}$ from $q$ to the point in space where you want to know $\bfvec{B}$;
2. Write $\bfvec{r}$ in the form $\bfvec{r}=r_x\ihat+r_y\jhat$; then
3. $\rhat=\bfvec{r}/r$, where $r=\sqrt{r_x^2+r_y^2}$.

The magnitude of $\bfvec{B}$ is

$$
B = \frac{\mu_o}{4\pi}\frac{|q|v\sin\phi}{r^2}
$$

where $\phi$ is the angle between $\bfvec{v}$ and $\bfvec{r}$ and $0 \le\phi \le 180^{\circ}$. If this formula is used, the direction can be found using the right--hand rule provided that $\bfvec{v}$ and $\bfvec{r}$ in the same cartesian coordinate plane (e.g., $x$--$z$ plane).

# Example I

If $q$ is at $(x,y)=(-a,-a)$ and is moving with $\bfvec{v}=v_o\ihat$, find the magnetic field at $(x,y)=(a,a)$.

**Solution**

To find $\hat{\mathbf{r}}$, we draw a vector from $q$ to the point where we want to compute $\bfvec{B}$. Based on the diagram, $r = 2\sqrt{2}a$ and $\bfvec{r}=2a\ihat + 2a\jhat$, so

$$\hat{\mathbf{r}}=\frac{\bfvec{r}}{r} = \left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right]$$

The cross product $\bfvec{v}\times\hat{\mathbf{r}}$ is

$$v_o\ihat\times\left[\frac{1}{\sqrt{2}}\ihat + \frac{1}{\sqrt{2}}\jhat\right] = \frac{v_o}{\sqrt{2}}(\ihat\times\jhat) = \frac{v_o}{\sqrt{2}}\khat$$

Thus,

$$\bfvec{B} = \frac{\mu_o}{4\pi}\frac{q\bfvec{v}\times\hat{\mathbf{r}}}{r^2} =  \frac{\mu_o}{4\pi} \frac{qv_o}{(8\sqrt{2})a^2}\khat$$

and 

$$B = \left|\frac{\mu_o}{4\pi} \frac{qv_o}{(8\sqrt{2})a^2}\khat\right|=\frac{\mu_o}{4\pi} \frac{|q|v_o}{(8\sqrt{2})a^2}$$



