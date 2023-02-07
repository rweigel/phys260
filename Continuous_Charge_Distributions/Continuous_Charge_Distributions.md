```mdextension
title: Continuous Charge Distributions
```

# Overview

Previously, you found the electric field at a location in space due to more than one point charge by finding the electric field due to each charge and then vectorially summing the fields to get the total field (this is "using superposition").

This process requires a significant amount of calculation if there are many charges. To reduce the number of calculations when charges are closely spaced, we sometimes assume they are continuously distributed; in this case, to compute the electric field, we need to evaluate an integral rather than a sum with many terms.

[Section 21.5](https://drive.google.com/file/d/1JS_pBuNEwXdz9IzpSBFPJffgVacZmqN7/view?usp=sharing_remove_) of the textbook gives three examples of finding $\bfvec{E}$ for charges that are continuously and uniformly distributed: 1. along a straight line, 2. on a circle, and 3. on a disk. If you read the textbook examples and the lecture notes, you should be able to identify the following steps (not necessarily in this order).

1. Identify answer features (e.g., what should the direction of your final answer for $\bfvec{E}$ be?).
2. Find $d\bfvec{E}$ (or $dE$ and its direction) for a $dQ$ on the charged object. Use a diagram to check the direction.
3. Find $dQ$ in terms of coordinates (e.g., $dx$, $dy$, $r$, $d\theta$, etc.).
4. Simplify $d\bfvec{E}$ (if possible) using symmetry arguments.
5. Integrate $d\bfvec{E}$.
6. Check answer features.

In this activity, you will explicitly address all of these steps for charges that are uniformly and continuously distributed along a straight line.

# Finite Line of Charge

The following diagram shows a differential charge $dQ$ located on the $x$--axis. Recall that the general equation for the electric field due to a point charge (with $q$ replaced with $dQ$ and $\bfvec{E}$ replaced with $d\bfvec{E}$) is

$\displaystyle d\mathbf{E} =k\frac{dQ}{r^2}\hat{\mathbf{r}}$, which has magnitude $\displaystyle dE = k\frac{dQ}{r^2}$

(In a previous activity, you found the components of $\bfvec{E}$ using two methods that are used in the textbook. You may use either method for this problem.)

   \ifsolutions
   <img src="figures/Finite_Line.svg" width="25%"/>
   \else

   \newpage

   <img src="figures/Finite_Line.svg" width="100%"/>
   \fi

1. Draw the expected directions of $dE_x$ and $dE_y$ at a location on the $+y$--axis on the diagram given the location of $dQ$ shown on the figure (assume $dQ$ is positive).

2. In the diagram, the differential charge $dQ$ is at a positive $x$. At the same location on the $+y$--axis, draw the expected direction, using dotted lines for $dE_x$ and $dE_y$, if $dQ$ is at $-x$. 

   \ifsolutions
   **Solution**

   <img src="figures/Finite_Line-Solution.svg" width="50%"/>
   \fi

3. Based on your diagrams, do you expect any component of the electric field due to $dQ$ at $+x$ will cancel that due to $dQ$ at $-x$?

   \ifsolutions
   **Answer**: Yes, the $x$ components will cancel leaving a total field in the $+y$ direction.
   \fi

4. Find equations for the electric field components $dE_x$ and $dE_y$ at any location on the $y$--axis in terms of $dQ$, $x$, $y$, and $k$. 

   \ifsolutions
   **Solution**

   See the textbook for an alternative way of arriving at the same result.

   The vector from $dQ$ to a point on the $y$--axis is $\mathbf{r}=-x\ihat+y\jhat$. We need to find $\ds d\mathbf{E} = (k{dQ}/{r^2})\hat{\mathbf{r}}$, which can be written as $\ds d\mathbf{E}=( k{dQ}/{r^3})\mathbf{r}$ using $\rhat=\mathbf{r}/r$. This equation allows us to bypass the need to compute $\rhat$ explicitly. Using this and $\mathbf{r}$ from above gives

   $$d\mathbf{E} = k\frac{dQ}{r^3}\mathbf{r} = k\frac{dQ}{(\sqrt{x^2+y^2})^3}(-x\ihat+y\jhat)$$

   Thus,
    
   $$\ds dE_x = -k\frac{xdQ}{(\sqrt{x^2+y^2})^3}\qquad dE_y = k\frac{ydQ}{(\sqrt{x^2+y^2})^3}$$
   \else
   
   \newpage

   \fi

5. Suppose the charge $dQ$ is at $x=a$ and you want to know the electric field at $y=a$. Plug these values into your equations for $dE_x$ and $dE_y$. Are the signs of $dE_x$ and $dE_y$ consistent with what you drew for part 1.? Repeat supposing the charge $dQ$ is at $x=-a$ and you want to know the electric field at $y=a$. Are the signs of $dE_x$ and $dE_y$ for this $dQ$ consistent with what you drew for part 2.? 

   \ifsolutions
   \else
   <div style="height:3em"/>
   \fi

6. If the differential charge $dQ$ is at $x=0$, do you expect $dE_x$ or $dE_y$ to be zero? Is your answer consistent with the result of plugging in $x=0$ into your equations for $dE_x$ and $dE_y$?

   \ifsolutions
   \else
   <div style="height:3em"/>
   \fi

If the charge per unit length on the line is $\lambda$, then we can write $dQ=\lambda dx$. To find $E_x$ and $E_y$, integrate $dE_x$ and $dE_y$ from $x=-a$ to $a$.

7. Write down the integrals that must be evaluated to find $E_x$ and $E_y$. Do you expect either of the integrals to be zero? 

   \ifsolutions
   **Solution**

   $$E_x = -\int_{-a}^{a} k\frac{x\lambda dx}{(\sqrt{x^2+y^2})^3}$$

   $$E_y = \int_{-a}^{a} k\frac{y\lambda dx}{(\sqrt{x^2+y^2})^3}=ky\int_{-a}^{a} \frac{\lambda dx}{(\sqrt{x^2+y^2})^3}$$

   Based on 2., we expect $E_x$ to be zero. Mathematically, the integrand for $E_x$ is an odd function on the integration integral, which is another justification for $E_x$ being zero. (The integrand for $E_y$ is even, so we could change its limits to $0$ to $a$ and multiply by this integral by 2.)

   Note that with respect to integration, $y$ can be treated as a constant because the integration is with respect to $x$, which is why $y$ was factored out from the integral for $E_y$.
   \else
   <div style="height:8em"/>
   \fi

8. From an integral table (or using trig substitutions), we know $\displaystyle \int \frac{du}{(u^2+a^2)^{3/2}} = \frac{u}{a^2\sqrt{u^2+a^2}} + C$. Use this to find $E_y$.

   \ifsolutions
   **Solution**

   In class, you were shown how to use trig substitution. Here we use an integral identity from a table. Replacing the integration variable $u$ with $x$ and the constant $a$ with $y$, the identity can be written as

   $\displaystyle \int \frac{dx}{(x^2+y^2)^{3/2}} = \frac{x}{y^2\sqrt{x^2+y^2}} + C$

   We need to evaluate

   $$E_y = ky\lambda \int_{-a}^{a} \frac{dx}{(\sqrt{x^2+y^2})^3}$$

   Using the identity,

   $$E_y = ky\lambda \left[\frac{x}{y^2\sqrt{x^2+y^2}}\right]_{x=-a}^{x=a}=ky\lambda \frac{2a}{y^2\sqrt{a^2+y^2}}=\frac{2k\lambda a}{y}\frac{1}{\sqrt{a^2+y^2}}$$
   \else

   \newpage

   \fi

9. If $y$ is negative (for example, $y=-a$), is your answer for $E_y$ positive or negative? Is this consistent with what you expect based on the given diagram?

   \ifsolutions
   **Answer**: At points on the $-y$ axis, we expect the electric field to be downwards because if the line is positively charged, the electric field due to each $dQ$ on the line will be downwards. Plugging in $y=-a$ gives a negative $E_y$, as expected.
   \else
   <div style="height:3em"/>
   \fi

10. The total charge on the line is $Q=2a\lambda$ (length $\times$ charge/length). Suppose $y\gg a$ so you can replace $a^2+y^2$ with $y^2$. Is your equation for $E_y$ consistent with the electric field for a point charge $Q=2a\lambda$ at the origin?

   \ifsolutions
   **Answer**

   $$E_y = \frac{2k\lambda a}{y}\frac{1}{\sqrt{a^2+y^2}} =  \frac{kQ}{y}\frac{1}{\sqrt{a^2+y^2}} \simeq  \frac{kQ}{y}\frac{1}{\sqrt{y^2}}=\frac{kQ}{y}\frac{1}{|y|}$$

   If $y$ is positive, $E_y=kQ/y^2$, which is positive. If $y$ is negative, $E_y=-kQ/y^2$, which negative. (The textbook considers only the positive case, but given the above questions, it seems natural to ask this question.)
   \else
   <div style="height:6em"/>
   \fi

# Long Line of Charge

Using the result of the previous problem, we can find $E_y$ when $a \gg y$, which corresponds to a long line of charge. The result is

$$E_y=\frac{2\lambda k}{y}$$

This equation can be generalized to apply to any long, straight, and uniformly charged line of charge:

$$E=\frac{2\lambda k}{r}$$

where $r$ is the perpendicular distance from the line. The direction of $\bfvec{E}$ is perpendicular to the line with a direction that depends on the sign of the charge density $\lambda$: if $\lambda$ is positive, $\bfvec{E}$ points away from the line; if $\lambda$ is negative, $\bfvec{E}$ points towards the line.

A long line of charge lies along the line $y=b$.

1. Find the electric field magnitude and direction at the origin.

   \ifsolutions
   **Answer**

   $\ds E=\frac{2\lambda k}{b}$, direction downwards, or $\ds \bfvec{E}=-\frac{2\lambda k}{b}\jhat$
   \else
   <div style="height:6em"/>
   \fi

2. Find the electric field magnitude and direction at $(x,y)=(b,0)$.

   \ifsolutions
   **Answer** Same as 1. For a long line of charge, the electric field is always perpendicular to the line; the field due to a long line of charge depends only on the perpendicular distance to the line, which is the same here as in part 1.
   \fi
