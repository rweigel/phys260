# Overview

When using Gauss’s law, one needs to draw an imaginary volume in space and compute how much charge is inside the volume.

In general, the imaginary volume that is used is one for which computation of the electric flux is easy. That is, the imaginary volume will be such that the electric field is either parallel or perpendicular to all parts of the surface.

In this activity, you are given the imaginary surface. To use Gauss's law, one must identify the imaginary surface that will allow for an easy calculation of the electric flux; this is covered in a separate activity.

# Line of Charge

A total of $+3Q$ is uniformly distributed a line of length $L$. The blue Gaussian cylinder shown has a length $l$, radius $r$, and the same center line as the insulator.

<img src="figures/Line.svg"/>

1. Find the charge density on the line.

    {\bf Answer}: Because the charge is uniformly distributed on the line, the the charge density is the total charge divided by the length: $\lambda={3Q}/{L}$.

2. Find the amount of charge enclosed by the Gaussian cylinder when it has radii of $r=l/100$, $r=l/2$, $r=l$, and $r=2l$. The enclosed charge should be in terms of one or more of $\epsilon_o$, numbers, and the parameters given ($Q$, $L$, $l$).

    {\bf Answer}:  The dashed line in the figure is the part of the line inside of the Gaussian cylinder. The length of the dashed line is $l$. The charge enclosed for all four cases is $Q_{\text{encl}}=\lambda l=3Q{l}/{L}$. In retrospect, one could have obtained this equation without considering the charge density -- the charge enclosed is the total charge $\times$ the ratio $l/L$. 

    The equation for the charge enclosed does not depend on the radius of the Gaussian cylinder. Visually, this is expected. If the radius of the cylinder increases, the length of the line inside of the cylinder does not change. 

    Check: As $l\rightarrow 0$, we expect from the diagram that the amount of charge enclosed should approach zero. This equation also says that as the ratio $l/L\rightarrow 0$, $Q_{\text{encl}}\rightarrow 0$. Does this make sense?

3. Plot the four values of enclosed charge calculated above versus the radius of the Gaussian cylinder. 

    {\bf Answer:}

    <img src="figures/Line_Graph.svg"/>

4. Find an equation that relates $Q_{\text{encl}}$ to $r$. Plot this equation on the graph above.

    {\bf Answer}: As noted in the answer to part 2., the enclosed charge does not change as the radius of the Gaussian cylinder changes. So $Q_{\text{encl}}(r)=\lambda h=\text{const}$, corresponding to the straight line on the graph.

\newpage

# Cylindrical Shell

A hollow cylinder of radius $R$ and length $H$ has a charge of $+3Q$ distributed _on its curved surface_. The blue Gaussian cylinder shown has a length $h$ and radius $r$ and has the same center line ("coaxial") as the charged cylinder.

<img src="figures/Hollow_Cylinder.svg"/>

1. Find the surface charge density on the curved part of the insulating cylinder. Also find the charge per unit length on the curved part of the insulating cylinder.

    {\bf Answer}: The area of the curved surface is the circumference $\times H = 2\pi RH$. The charge is uniformly distributed, so the charge density is the total charge divided by the area: $\sigma={3Q}/{2\pi RH}$. The length of the cylinder is $H$, so the linear charge density is $\lambda = 3Q/H$. Note that $\lambda=\sigma 2\pi R$.

2. Find the amount of charge enclosed in Gaussian cylinder of radii $r=0$, $r=R/2$, $r=2R$, and $r=4R$.

    {\bf Answer}: Imagine that the blue Gaussian cylinder was fully inside of the hollow cylinder. There would be no charge inside of it. As a result, the charge enclosed for $r=0$ and $r=R/2$ is zero. Once the Gaussian cylinder's radius is larger than the hollow cylinder's radius, the total charge inside of the Gaussian cylinder does not change. To find the charge enclosed in this case, we need to find the area of the hollow cylinder enclosed. It is $2\pi R h$. The charge enclosed is the charge density computed in part 1. times this area: $Q_{\text{encl}}=\sigma (2\pi R h) = 3Q{h}/{H}$. In retrospect, one could have obtained this equation without considering the surface charge density -- the charge enclosed is the total charge $\times$ the ratio $h/H$. 
    
    Alternatively, we can state that the amount of charge enclosed is the linear charge density $\times h = \lambda h = 3Q{h}/{H}$.

    Check: Visually, as the length $h$ of the Gaussian cylinder shrinks to zero, the enclosed charge should approach zero. The equation for $Q_{\text{\text{encl}}}$ is consistent with this observation.
    
3. Plot the four values of enclosed charge calculated above versus the radius of the Gaussian cylinder.

    {\bf Answer}: 

    \include{Gauss/figures/Cylindrical_Shell_and_Gaussian_Cylinder_Graph}

4. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r<R$. Plot this equation on the graph above.

    {\bf Answer}: The enclosed charge is zero for $r<R$, so $Q_{\text{\text{encl}}}(r)=0$.

5. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r>R$. Plot this equation on the graph above.

    {\bf Answer}: The enclosed charge is constant for $r>R$, so, $Q_{\text{\text{encl}}}(r)=3Q{l}/{L}=\text{constant}$.

\newpage

# Solid Cylinder

A solid insulating cylinder of radius, $R$ and length, $L$ has a charge of $+3Q$ uniformly distributed within it. The Gaussian cylinder shown has the same center line as the insulating cylinder, length $l$, and radius $r$.

Gauss/figures/Solid_Cylinder_and_Gaussian_Cylinder.png}

1. Find the charge density in the insulating cylinder.

    {\bf Answer:} The insulating cylinder is a volume. The volume of a cylinder is its cross-sectional area time its height, $\pi R^2 L$. The charge density is charge/volume, $\rho=3Q/(\pi R^2 L)$.

2. Find the amount of charge enclosed in a Gaussian cylinder of radius $r=0$, $r=R/2$, $r=2R$, and $r=4R$.

    {\bf Answer}: When $r<R$, the Gaussian cylinder is fully inside of the insulating cylinder. The charge in the Gaussian cylinder is the charge density of the insulating cylinder times the volume of the Gaussian cylinder: $Q_{\text{encl}}=\rho \pi r^2 l = 3Q(r^2/R^2)(l/L)$.

    For any $r\ge R$, the amount of charge inside the Gaussian cylinder does not change with $r$. The amount of charge depends on volume of insulator inside of the Gaussian cylinder, which is $\pi R^2 l$, so $Q_{\text{encl}}=\rho \pi R^2 l = 3Q(l/L)$. When $l=L$, $Q_{\text{encl}}=3Q$, which makes sense because all of the insulator is inside of the Gaussian cylinder.

3. Plot the four values of enclosed charge  calculated above versus the radius of the Gaussian cylinder.

    {\bf Answer}: For $r<R$, the curve will be a parabola because of the $r^2$. For $r>R$, curve will be a horizontal line that intersects with the parabola at $r=R$. For values outside of the cylinder, r $>$ R, the enclosed charge will be constant.

4. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r<R$. Plot this equation on the graph above.

    {\bf Answer}: As noted in part 2, the charge enclosed is $Q_{\text{encl}}=\rho \pi r^2 l = 3Q(r^2/R^2)(l/L)$. Because of the dependence on r$^2$ the curve is parabolic. 

5. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r>R$. Plot this equation on the graph above.

    {\bf Answer}: As noted in part 2, the charge enclosed is $Q_{\text{encl}}=3Q$ so it is constant. 

\newpage

# Spherical Shell

An insulating sphere of radius $R$ has a charge of $+3Q$ distributed \emph{on its surface}. The cross-section of the sphere is shown along with a dashed line representing the surface of a Gaussian sphere, which has the same center as the charged sphere and a radius $r$.

Gauss/figures/Spherical_Shell_with_Gaussian_Sphere}

1. Find the surface charge density on the insulating sphere.

    {\bf Answer}: $\sigma = 3Q/4\pi R^2$

2. Find the amount of charge enclosed in Gaussian sphere of radii $r=0$, $r=R/2$, $r=2R$, and $r=4R$.

    {\bf Answer}: When $r < R$, $Q_{\text{encl}}=0$. When $r\ge R$, $Q_{\text{encl}}=3Q$ because all of the charge is enclosed.

3. Plot the four values of enclosed charge calculated above versus the radius of the Gaussian sphere.

4. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r<R$. Plot this equation on the graph above. 

    {\bf Answer}: $Q_{\text{encl}}=0$

5. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r>R$. Plot this equation on the graph above.

    {\bf Answer}: Plot should be a horizontal line between $r$ and $R$ at y = 0 and a horizontal line for $r\ge R$ at y = $3Q$.

\newpage

# Solid Sphere

An insulating sphere of radius $R$ has a charge of $+3Q$ distributed uniformly _throughout_ it. The cross--section of the sphere is shown along with a dashed line representing the surface of a Gaussian sphere, which has the same center as the charged sphere and a radius $r$.

1. Find the charge density in the sphere.

2. Find the amount of charge enclosed in Gaussian sphere of radii $r=0$, $r=R/2$, $r=2R$, and $r=4R$.

3. Plot the four values of enclosed charge calculated above versus the radius of the Gaussian sphere.

4. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r<R$. Plot this equation on the graph above.

5. Find an equation that relates $Q_{\text{encl}}$ and $r$ for %$r>R$. Plot this equation on the graph above.

\newpage

# Large Sheet

An insulator in the form of a square sheet with side length $L$ has a charge of $+3Q$ distributed uniformly on it. The blue Gaussian cylinder has a height $h$ and radius $r$ and half of it is above the sheet.

Gauss/figures/Plane_and_Gaussian_Cylinder.png

1. Find the charge density on the sheet.

    {\bf Answer}: $\sigma=3Q/L^2$

2. Find the amount of charge enclosed in Gaussian cylinder of radii $r=0$, $r=R/2$, $r=2R$, and $r=4R$.

    {\bf Answer}: As noted in class, no $R$ was given in the problem statement. The question should have asked for the charge enclosed for $r=L/32$, $r=L/16$, $r=L/8$, $r=L/4$. We are not interested in larger $r$ because Gauss's law can't be used unless the Gaussian cylinder is small relative to the sheet. This is discussed in the large sheet solution in the next section.

    The amount of charge enclosed for $r<L$ is $Q_{\text{encl}}=\sigma \pi r^2 = 3Q r^2/L^2$.

3. Plot the four values of enclosed charge calculated above versus the radius of the Gaussian cylinder.

4. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r<R$. Plot this equation on the graph above.

5. Find an equation that relates $Q_{\text{encl}}$ and $r$ for $r>R$. Plot this equation on the graph above.

    {\bf Answer}: The line should be a parabola that passes through the origin.
