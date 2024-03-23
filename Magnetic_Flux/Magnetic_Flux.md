# Introduction

The definition of magnetic flux is

$$\Phi_B = \int \mathbf{B}\cdot d\mathbf{A}$$

When the magnitude and direction of $\bfvec{B}$ is the same at all points on the surface, the integral simplifies to 

$$\Phi_B = \mathbf{B}\cdot \mathbf{A}$$

or, equivalently,

$$\Phi_B = BA\cos\phi$$

where $\theta$ is the angle between the $\bfvec{B}$ and $\bfvec{A}$ vectors.

Note that previously electric flux was covered. The same techniques that apply to computing electric flux apply to magnetic flux.See the Electric Flux activity for additional discussion.

# Computing $\Phi_B$

In the following figure, a square loop of area $A$ that can be rotated about the $z$ axis is shown. Assume that the normal direction of the loop is as shown in the diagram. A uniform external magnetic field points in the $\jhat$ direction.

<img src="figures/Square_I.svg"/>

1. At what angles in the range of $\phi=[0,360^\circ]$ is the magnetic flux zero?

2. Draw the loop, $\hat{\mathbf{n}}$, and $\bfvec{B}_{\text{ext}}$ as they would appear when viewed from large $z$ when $\phi=0^\circ$, $\phi=45^\circ$, $\phi=135^\circ$, and $\phi=180^\circ$.

3. When $\phi=45^\circ$, is the magnetic flux positive or negative? What is its value in terms of $B_oA$?

4. When $\phi=135^\circ$, is the magnetic flux positive or negative? What is its value in terms of $B_oA$?

5. Sketch a plot of the magnetic flux, $\Phi$, as a function of $\phi$.

{\bf Answer}:

1. The magnetic flux will be zero when the normal vector is perpendicular to  $\bfvec{B}_{\text{ext}}$. This corresponds to $\phi = 90^\circ$ and $\phi = 270^\circ$

2. &nbsp;

   <img src="figures/Square_I_Solution_A.svg"/>

3. As shown in the diagram, the dot product of the normal vector and $\mathbf{B}_{\text{ext}}$ will be positive when $\phi=45^\circ$, so the flux will be positive. Its value will be $B_oA\cos 45^\circ=B_oA/\sqrt{2}$.

4. As shown in the diagram above, when $\phi=135^\circ$ the dot product of the normal vector and $\mathbf{B}_{\text{ext}}$ will be negative, so the flux will be negative. Its value will be $B_oA\cos 135^\circ=-B_oA\cos 45^\circ=-B_oA/\sqrt{2}$.

5. The curve is $\Phi=B_oA\cos\phi$ is sketched below along with dots that were used to help determine the shape of the curve.

   <img src="figures/Square_I_Solution_B.svg"/>

# Computing $d\Phi_B/dt$

The time rate of change of magnetic flux through a closed loop is a quantity that will be used when Faraday's law is covered.

Suppose the loop in the previous problem rotates at a constant rate.

1. At what angles is $d\Phi_B/dt=0$?
2. For what angle range is $d\Phi_B/dt$ increasing?
3. For what angle range is $d\Phi_B/dt$ decreasing?
4. What is the formula for $d\Phi_B/dt$?





