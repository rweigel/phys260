# Overview

When using Gauss’s law, one needs to draw an imaginary volume in space and compute how much charge is inside the volume.

In general, the imaginary volume that is used is one for which computation of the electric flux is easy. That is, the imaginary volume will be such that the electric field is either parallel or perpendicular to all parts of the surface.

In this activity, you are given the imaginary surface. To use Gauss's law, one must identify the imaginary surface that will allow for an easy calculation of the electric flux; this is not covered in this activity.

# Line of Charge

A total of $+3Q$ is uniformly distributed a non--conducting line of length $L$. The blue Gaussian cylinder shown has a length $h$, radius $r$, and the same center line as the charged line.

<img src="figures/Line.svg"/>

1. Find the linear charge density, $\lambda$, on the line.

    {\bf Answer}: Because the charge is uniformly distributed on the line, the the charge density is constant and is the total charge divided by the length: $\lambda={3Q}/{L}$.


2. Find an equation that relates $Q_{\text{encl}}$ to $r$ in terms of $\lambda$ and one or more of $r$, $h$, and $L$.

    {\bf Answer}: As noted in the answer to part 2., the enclosed charge does not change as the radius of the Gaussian cylinder changes. So $Q_{\text{encl}}(r)=\lambda h=\text{const}$, corresponding to the straight line on the graph in the answer to part 3.

    {\bf Answer}:  The dashed line in the figure is the part of the line inside of the Gaussian cylinder. The length of the dashed line is $h$. The charge enclosed for all four cases is $Q_{\text{encl}}=\lambda h=3Q{h}/{L}$. In retrospect, one could have obtained the latter equation without considering the charge density -- the charge enclosed is the total charge $\times$ the ratio $h/L$.


3. Find the amount of charge enclosed by the Gaussian cylinder when it has radii of $r=h/100$, $r=h/2$, $r=h$, and $r=2h$.


4. Plot the four values of enclosed charge calculated above versus the radius of the Gaussian cylinder. 

    {\bf Answer:}

    <img src="figures/Line_Graph.svg"/>

\newpage

# Cylindrical Shell

A non--conducting hollow cylinder of radius $R$ and length $H$ has a charge of $+3Q$ distributed _on its curved surface_. The blue Gaussian cylinder shown has a length $h$ and radius $r$ and has the same center line as the charged cylinder.

<img src="figures/Hollow_Cylinder.svg"/>

1.  Find the linear charge density, $\lambda$, of the charged cylinder.

    {\bf Answer}: The length of the cylinder is $H$, so the linear charge density is $\lambda = 3Q/H$.

2. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r<R$. Your equation should involve $\lambda$ and one or more of $h$, $r$, and $R$.

    {\bf Answer}: Imagine that the blue Gaussian cylinder was fully inside of the hollow cylinder. There would be no charge inside of it. As a result, the charge enclosed for $r< R$ is zero, so $Q_{\text{encl}}=0$.

3. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r>R$. Your equation should involve $\lambda$ and one or more of $h$, $r$, and $R$.

    The amount of charge enclosed is the charge per unit length $\times h = \lambda h$, so  $Q_{\text{encl}}=\lambda h$. (The amount of charge enclosed does not depend on $r$.)

4. Find the amount of charge enclosed by the Gaussian cylinder when it has radii of $r=0$, $r=R/2$, $r=2R$, and $r=4R$.


5. Plot the four values of enclosed charge calculated above versus the radius of the Gaussian cylinder. Plot the equations found in parts 2. and 3.

\newpage

# Solid Cylinder

A non--conducting solid cylinder of radius, $R$ and length, $L$ has a charge of $+3Q$ uniformly distributed within it. The Gaussian cylinder has length $h$, radius $r$, and the same center line as the charged cylinder.

<img src="figures/Solid_Cylinder.svg"/>

1. Find the volume charge density, $\rho$, of the charged cylinder.

    {\bf Answer:} The volume of the charged cylinder is its cross-sectional area time its height: $V=\pi R^2 h$. The charge density is charge/volume: $\rho=3Q/(\pi R^2 L)$.

2. Find the amount of charge enclosed in a Gaussian cylinder of radius $r=0$, $r=R/2$, $r=2R$, and $r=4R$.

    {\bf Answer}: When $r<R$, the Gaussian cylinder is fully inside of the charged cylinder. The charge in the Gaussian cylinder is the charge density of the charged cylinder times the volume of the Gaussian cylinder: $Q_{\text{encl}}=\rho \pi r^2 h = 3Q(r^2/R^2)(h/H)$.

    For any $r\ge R$, the amount of charge inside the Gaussian cylinder does not change with $r$. The amount of charge depends on volume of inside of the Gaussian cylinder, which is $\pi R^2 h$, so $Q_{\text{encl}}=\rho \pi R^2 h = 3Q(h/H)$. When $h=H$, $Q_{\text{encl}}=3Q$, which makes sense because all of the charge is inside of the Gaussian cylinder.

3. Plot the four values of enclosed charge  calculated above versus the radius of the Gaussian cylinder.

    {\bf Answer}: For $r<R$, the curve will be a parabola because of the $r^2$. For $r>R$, curve will be a horizontal line that intersects with the parabola at $r=R$. For values outside of the cylinder, $r>R$, the enclosed charge will be constant.

4. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r<R$. Plot this equation on the graph above.

    {\bf Answer}: As noted in part 2, the charge enclosed is $Q_{\text{encl}}=\rho \pi r^2 h$. Because of the dependence on r$^2$, the curve is a parabola. 

5. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r>R$. Plot this equation on the graph above.

    {\bf Answer}: As noted in part 2, the charge enclosed is $Q_{\text{encl}}=\rho \pi R^2 h$ so it is independent of $r$. 

\newpage

# Spherical Shell

A non--conducting spherical shell of radius $R$ has a charge of $+3Q$ distributed _on its surface_. The cross-section of the sphere is shown along with a dashed line representing the surface of a Gaussian sphere, which has the same center as the charged sphere and a radius $r$.

1. Find the surface charge density on the sphere.

    {\bf Answer}: $\sigma = 3Q/4\pi R^2$

2. Find the amount of charge enclosed in Gaussian sphere of radii $r=0$, $r=R/2$, $r=2R$, and $r=4R$.

    {\bf Answer}: When $r < R$, $Q_{\text{encl}}=0$. When $r\ge R$, $Q_{\text{encl}}=\sigma 4\pi R^2=3Q$ because all of the charge is enclosed.

3. Plot the four values of enclosed charge calculated above versus the radius of the Gaussian sphere.

4. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r<R$. Plot this equation on the graph above. 

    {\bf Answer}: $Q_{\text{encl}}=0$

5. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r>R$. Plot this equation on the graph above.

    {\bf Answer}: $Q_{\text{encl}}=\sigma 4\pi R^2$, which corresponds to a horizontal line that intersects the parabola at $r=R$.

\newpage

# Solid Sphere

A non--conducting sphere of radius $R$ has a charge of $+3Q$ distributed uniformly _throughout_ it. The cross--section of the sphere is shown along with a dashed line representing the surface of a Gaussian sphere, which has the same center as the charged sphere and a radius $r$.

1. Find the volume charge density, $\rho$, of the charged sphere.

    {\bf Answer}: $\ds \rho=3Q/[(4/3)\pi R^3]$

2. Find the amount of charge enclosed in Gaussian sphere of radii $r=0$, $r=R/2$, $r=2R$, and $r=4R$.

    {\bf Answer}: For $r \le R$, $Q_{\text{encl}}=\rho [(4/3)\pi r^3]$
    
    For $r \ge R$,  $Q_{\text{encl}}=\rho [(4/3)\pi R^3]$

3. Plot the four values of enclosed charge calculated above versus the radius of the Gaussian sphere.

4. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r<R$. Plot this equation on the graph above.

5. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r>R$. Plot this equation on the graph above.

\newpage

# Large Sheet

<img src="figures/Sheet.svg"/>

A non--conducting square sheet with side length $L$ has a charge of $+3Q$ distributed uniformly on it. The blue Gaussian cylinder has a height $h$ and radius $r$ and half of it is above the sheet.

1. Find the charge density on the sheet.

    {\bf Answer}: $\sigma=3Q/L^2$

2. Find the amount of charge enclosed in Gaussian cylinder of radii $r=L/32$, $r=L/16$, $r=L/8$, $r=L/4$. (In Gauss's law problems, $L$ is much larger than $r$, so we do not need to consider cases of $r > L$.)

    {\bf Answer}: The amount of charge enclosed for $r<L$ is $Q_{\text{encl}}=\sigma \pi r^2 = 3Q r^2/L^2$.

3. Plot the four values of enclosed charge calculated above versus the radius of the Gaussian cylinder.

4. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r<L$. Plot this equation on the graph above.
