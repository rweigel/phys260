```mdextension
title: Continous Charge Distributions
```

# Overview

Previously you have found the electric field at a location in space due to many point charges by finding the electric field due to each charge and then vectorially summing the fields to get the total field (this is "using superposition").

If there are many charges, this process requires a significant amount of calculation. To reduce the number of calculations when charges are closely spaced, we sometimes assume they are continuously distributed; in this case, to compute the electric field we need to evaluate an integral rather than a sum with many terms.

[Section 21.5](https://drive.google.com/file/d/1JS_pBuNEwXdz9IzpSBFPJffgVacZmqN7/view?usp=sharing_remove_) of the textbook gives three examples for charges that are continuously distributed:

1. charges uniformly distributed along a straight line,
2. charges uniformly distributed on a circle, and
3. charges uniformly distributed on a disk.

If you read the textbook examples and the lecture notes, you should be able to identify the following steps (not necessarily in this order).

1. Identify answer features
2. Find $d\bfvec{E}$ (or $dE$ and its direction) for a $dQ$ on the charged object
3. Find $dQ$ in terms of coordinates (e.g., $dx$, $dy$, $r$, $d\theta$, etc.)
4. Simplify $d\bfvec{E}$ (if possible) using symmetry arguments
5. Integrate $d\bfvec{E}$
6. Check answer features

In this activity, you will explicitly address all of these steps for charges that are uniformly and continuously distributed along a straight line.

# Finite Line of Charge

In the following diagram, a differential charge $dQ$ is shown at a location on the $x$--axis. Recall that the general equation for the electric field due to a point charge (with $q$ replaced with $dQ$ and $\bfvec{E}$ replaced with $d\bfvec{E}$) is

$\displaystyle d\mathbf{E} =k\frac{dQ}{r^2}\hat{\mathbf{r}}$, which has magnitude $\displaystyle dE = k\frac{dQ}{r^2}$

(In a previous activity, you found the components of $\bfvec{E}$ using two methods that are used in the textbook. You may use either method for this problem.)

\newpage

<img src="figures/Finite_Line.svg"/>

1. Draw the expected directions of $dE_x$ and $dE_y$ at a location on the $+y$--axis on the diagram given the location of $dQ$ shown on the figure (assume $dQ$ is positive).

    **Comment** In class, Patrick assumed a position of $b$ on the $y$--axis to avoid the confusion that sometimes arises with $y$ being a variable but a constant with respect to integration. Here we allow $y$ to be variable similar to the textbook example.

2. In the diagram, the differential charge is at a positive $x$. At the same location on the $+y$--axis, draw the expected direction of $dE_x$ and $dE_y$ on the diagram with dotted lines if $dQ$ is at $-x$. 

3. Draw the expected direction of $dE_x$ and $dE_y$ on the diagram at a location on the $-y$--axis for $dQ$ at the position in the figure. 

4. Find an equation for the electric field components $dE_x$ and $dE_y$ at any location on the $y$--axis in terms of $dQ$, $x$, $y$, and $k$. 

    **Solution**
    
    See the textbook for an alternative way of arriving at the same result.
    
    The vector from $dQ$ to a point on the $y$--axis is $\mathbf{r}=-x\ihat+y\jhat$.

    $$d\mathbf{E} = k\frac{dQ}{r^2}\hat{\mathbf{r}} = k\frac{dQ}{r^3}\mathbf{r}$$
    
    where in the last step, $\rhat=\mathbf{r}/r$ was used. Substitution gives

    $$d\mathbf{E} = k\frac{dQ}{(\sqrt{x^2+y^2})^3}(-x\ihat+y\jhat)$$

    Thus,
    
    $$\ds dE_x = -k\frac{xdQ}{(\sqrt{x^2+y^2})^3}\qquad dE_y = k\frac{ydQ}{(\sqrt{x^2+y^2})^3}$$

%<div style="height:8em"/>

5. Do your equations for $dE_x$ and $dE_y$ give the directions predicted by your answers to 1.--3.? Try plugging in values of $y=\pm a$ and $x=\pm a$.

<div style="height:3em"/>

6. If the differential charge $dQ$ is at $x=0$, do you expect $dE_x$ or $dE_y$ to be zero?

<div style="height:1em"/>

If the charge per unit length on the line is $\lambda$, then we can write $dQ=\lambda dx$. To find $E_x$ and $E_y$, we can integrate $dE_x$ and $dE_y$ from $x=-a$ to $a$.

7. Do you expect either of the integrals to be zero? Write down the integrals that must be evaluated to find $E_x$ and $E_y$. 

    **Solution**
    
    $$E_x = -\int_{-a}^{a} k\frac{x\lambda dx}{(\sqrt{x^2+y^2})^3}$$

    $$E_y = \int_{-a}^{a} k\frac{y\lambda dx}{(\sqrt{x^2+y^2})^3}=ky\int_{-a}^{a} \frac{\lambda dx}{(\sqrt{x^2+y^2})^3}$$

    Note that with respect to integration, $y$ can be treated as a constant because the integration is with respect to $x$, which is why $y$ can be factored out as done in the equation for $E_y$.

%<div style="height:1em"/>

8. From an integral table (or using trig substitutions), we know $\displaystyle \int \frac{du}{(u^2+a^2)^{3/2}} = \frac{u}{a^2\sqrt{u^2+a^2}} + C$. Use this to find $E_y$.

    **Answer**

    In class, you were shown how to use trig substitution. Here we use an integral identity from a table. Replacing the integration variable $u$ with $x$ and the constant $a$ with $y$, the identity can be written as

    $\displaystyle \int \frac{dx}{(x^2+y^2)^{3/2}} = \frac{x}{y^2\sqrt{x^2+y^2}} + C$

    We need to evaluate

    $$E_y = ky\lambda \int_{-a}^{a} \frac{dx}{(\sqrt{x^2+y^2})^3}$$

    Using the identity, this is

    $$E_y = ky\lambda \left[\frac{x}{y^2\sqrt{x^2+y^2}}\right]_{x=-a}^{x=a}=ky\lambda \frac{2a}{y^2\sqrt{a^2+y^2}}=\frac{2k}{y}\frac{1}{\sqrt{a^2+y^2}}$$

\newpage

9. If $y$ is negative (for example $y=-a$), is $E_y$ positive or negative? Is this consistent with your answer to 3.?

%<div style="height:3em"/>

10. The total charge on the line is $Q=2a\lambda$ (length $\times$ charge/length). Suppose $y\gg a$ so that you can replace $y^2+a^2$ with $y^2$. Is your equation for $E_y$ consistent with the electric field for a point charge $Q=2a\lambda$ at the origin?

    **Answer**
    
    $$E_y = \frac{2k}{y}\frac{1}{\sqrt{a^2+y^2}} \simeq  \frac{2k}{y}\frac{1}{\sqrt{y^2}}=\frac{2k}{y}\frac{1}{|y|}$$

    If $y$ is positive, $E_y$ is positive. If $y$ is negative, $E_y$ is negative, as expected. (The textbook considers the limit with $y$ positive only, but given the questions asked above, it seems natural to ask this question.)

%<div style="height:3em"/>

# Long Line of Charge

Using the result of the previous problem, we can find $E_y$ when $a \gg y$, which corresponds to a long line of charge. The result is

$$E_y=\frac{2\lambda k}{y}$$

This equation can be written more generally as

$$E=\frac{2\lambda k}{r}$$

where $r$ is the perpendicular distance from the line and the electric field $E$ direction is perpendicular the line with a direction that depends on the sign of the charge density $\lambda$.

A long line of charge lies along the line $y=b$.

1. Find the electric field magnitude and direction at the origin.

    **Answer**

    $\ds E=\frac{2\lambda k}{b}$, direction downwards, or $\ds \bfvec{E}=-\frac{2\lambda k}{b}\jhat$

%<div style="height:8em"/>

2. Find the electric field magnitude and direction at $(x,y)=(b,0)$.

    **Αnswer** Same as 1.
