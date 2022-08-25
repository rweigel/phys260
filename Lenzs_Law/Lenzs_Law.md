# Lenz's Law (Ch 29)

## Introduction

In this section we get our first look at the connection between magnetic and electric fields. A changing magnetic flux can {\it induce} the flow of a current in a conducting loop. 

As a reminder, the general equation for magnetic flux is:

$$
\Phi_B = \int \mathbf{B}\cdot d\mathbf{A}
$$

If the magnitude (strength) of the magnetic field is not changing and the angle between the magnetic field vector and the area vector doesn't change over the surface, then integration is not required and we can write

$$
\Phi_B = \mathbf{B}\cdot \mathbf{A}
$$

or, equivalently,

$$
\Phi_B = BA\cos\phi
$$

See the previous tutorial for examples that demonstrate the use of this equation.

There are three ways in which flux can change:

1.  The magnitude of $\mathbf{B}$ can change. To do this, a magnet can be moved closer or farther away from a conducting loop, a loop can be moved closer or farther away from a magnet, or the current in the loop that is generating the magnetic field can be changed. See Example 29.1 in the textbook for an example of the creation of a changing magnetic field without a magnet.
    
2.  The area $A$ can change. To do this, the loop cross-section can be expanded or contracted, either by heating or cooling a wire or, more commonly, using a device called a slidewire generator (see Example 29.5).
    
3.  The angle can change. To do this, a conducting loop can be rotated (see Example 29.3). This is important in motors. 

In this tutorial, you will first determine the direction of the induced current using Lenz's law. After becoming familiar with the direction of the induced current, we will use Faraday's law to explore the induced emf that drives the induced current. 

Lenz's law follows from Faraday's law. In principle, Faraday's law with careful attention paid to signs can be used to determine the direction of induced current, in which case Lenz's law is not needed. In a similar way that using the right--hand rules to get the general direction for force can be used to check your math on a cross-product, Lenz's Law provides a check on the direction of the induced current when using Faraday's law. 

## Lenz's Law

As described in the textbook,

{\bf Lenz’s Law:} The direction of any magnetic induction effect is such as to oppose the cause of the effect.

Here, we'll use a simpler definition.

{\bf Lenz’s Law alternative}: When the external magnetic flux through a conducting loop changes, a current appears (is induced) in the loop. This induced current creates an induced magnetic field. The direction of the induced current is such that the magnetic field it creates attempts to keep the magnetic flux unchanged.

## Example 2.1

A spatially uniform external magnetic field points out of the page and its magnitude is increasing in time.

Assume that the area vector, which is normal to the gray cross-sectional area of rectangular conducting loop, is out of the page.

\input{EMF and Induced Fields/figures/Square_Loop_I}

1.  Is the magnetic flux through the loop increasing or decreasing? 

2.  What is the direction of an induced magnetic field, through the gray region, that will counteract the change in the magnetic flux? Is the direction of the induced magnetic field positive or negative?

3.  What would the direction of the current in the loop have to be to induce a magnetic field in the direction you got in part b? This is the direction of the induced current.  

4.  If you assume that the normal direction of the cross-sectional area of loop is into the page, will your answers change?

{\bf Answer}:

1.  The magnetic field is in the same direction of as the normal, so $\Phi_B=\mathbf{B}_{ext}\cdot \mathbf{A}=\mathbf{B}_{ext}\cdot A\hat{\mathbf{n}}$ is positive. The flux is increasing. 

2.  A \emph{induced} magnetic field, that counteracts the increasing magnetic flux, would have to be pointed into the page. A magnetic field that counteracts the increasing magnetic flux would be in the negative direction.

3.  By the right-hand rule, to create a magnetic field into the page would require a clockwise current.

4.  The sign of the magnetic fluxes will change but the current direction that follows from Lenz's law will be the same.

## Problem

A spatially uniform external magnetic field points into of the page and its magnitude is decreasing in time.

Assume that the normal direction of the cross-sectional area of loop is out of the page.

\input{EMF and Induced Fields/figures/Square_Loop_II}

1.  Is the magnetic flux through the loop increasing or decreasing? 

2.  What direction would an induced magnetic field have to be to oppose the change in the magnetic flux? Would the direction of the induced magnetic field be positive or negative? 

3.  What would the direction of the current in the loop have to be to induce a magnetic field in the direction you got in part b? This is the direction of the induced current. 

4.  If you assume that the normal direction of the cross-sectional area of loop is into the page, will your answers change?

{\bf Answer}:

1.  The magnetic field is in the opposite direction of as the normal, so $\Phi_B=\mathbf{B}_{ext}\cdot \mathbf{A}=\mathbf{B}_{ext}\cdot A\hat{\mathbf{n}}$ is negative. However, the external magnetic field is decreasing with time so the magnetic flux is increasing (the magnetic flux is large an negative initially; because $B_{ext}$ is decreasing with time, after a short amount of time the flux is still negative but closer to zero). Another way of working this out is to consider the derivative of flux: $\Phi_B=-B_{ext}A$, $d \Phi_B/dt = -AdB_{ext}/dt$. Here $dB_{ext}/dt$ is given to be negative, so $\Phi_B/dt$ is positive. 

(b) A \emph{induced} magnetic field, that will create a flux that counteracts the increasing magnetic flux, would have to be pointed into the page. The induced magnetic flux is thus negative.

(c) By the right-hand rule, to create an induced magnetic field into the page requires a clockwise current.

(d) The sign of the magnetic fluxes will change but the current direction that follows from Lenz's law will be the same.

## Example 2.2

A spatially uniform external magnetic field points out of the page and it is not changing with time.

The conducting loop is heated causing the gray cross-sectional area to increase with time.

Assume that the normal direction of the gray cross-sectional area of loop is out of the page.

\input{EMF and Induced Fields/figures/Square_Loop_I}

1.  Is the magnetic flux through the loop increasing or decreasing? 

2.  What direction would an induced magnetic field have to be to oppose the change in the magnetic flux? Would the direction of the induced magnetic field be positive or negative? 

3.  What would the direction of the current in the loop have to be to induce a magnetic field in the direction you got in part b? This is the direction of the induced current. 

4.  If you assume that the normal direction of the cross-sectional area of loop is into the page, will your answers change?

{\bf Answer}:

1.  The magnetic flux is $\Phi_B=\mathbf{B}_{ext}\cdot \mathbf{A}=\mathbf{B}_{ext}\cdot A\hat{\mathbf{n}}$ = $B_{ext}A$. Here $A$ is increasing, so the magnetic flux is increasing.

2.  An induced magnetic field into the page will create a negative flux to counteract the increase in flux.

3.  A clockwise current creates a magnetic field into the page.

4.  The sign of the magnetic fluxes will change. The direction of current will not change.

## Problem

An external magnetic field points into of the page and it is not changing with time.

Assume that the normal direction of the cross-sectional area of loop is out of the page.

The conducting loop of area $A$ is cooled and as a result its cross-sectional area decreases with time.

\input{EMF and Induced Fields/figures/Square_Loop_II}

1.  Is the magnetic flux through the loop increasing or decreasing? 

2.  What direction would an induced magnetic field have to be to oppose the change in the magnetic flux? Would the direction of the induced magnetic field be positive or negative? 

3.  What would the direction of the current in the loop have to be to induce a magnetic field in the direction you got in part b? This is the direction of the induced current. 

4.  If you assume that the normal direction of the cross-sectional area of loop is into the page, will your answers change?

{\bf Answer}:

1.  The magnetic flux is $\Phi_B=\mathbf{B}_{ext}\cdot \mathbf{A}=\mathbf{B}_{ext}\cdot A\hat{\mathbf{n}}$. Here the magnetic field is in the opposite direction of the normal so $\mathbf{B}_{ext}\cdot A\hat{\mathbf{n}}$ is negative. The area $A$ is decreasing so the magnetic flux, which is initially negative, is increasing towards zero. 

2.  The induced magnetic field would have to be into the page. The induced magnetic field would be in the direction opposite of the chosen normal direction for the loop.

3.  By the right-hand rule, a clockwise current creates a magnetic field into the page. This direction of induced current is such that its associated induced magnetic field is attempting to keep the magnetic flux unchanged.

4.  The sign of magnetic fluxes will change, the direction of the current will not change.

%To understand the direction a current will be induced in a wire, one can start by considering the magnetic forces on charges on a conductor that is moving within the field. 

%Note: we will discuss later that this is only part of the explanation and cannot explain the motion of charges when the conductor is not moving (but the field is still changing). 

## Induced Currents and the Lorentz Force Law

Lenz's law can only be used to determine the direction a current will flow in response to a changing magnetic flux through a conducting loop. It does not explain why currents start to flow. The currents flow due to one of two forces. These forces are 

* The Lorentz force, which says that a charge moving in a magnetic field experiences a force according to $\mathbf{F}=q\mathbf{v}\times\mathbf{B}$. An example of this was given in Example 2.2 and 2.3. In both cases, the charges on the conductor are moving in a magnetic field and as a result, they will experience a Lorentz Force that initiates the flow of current.

* An induced electric field. In Example 2.1, the conductor is not moving and so its velocity is zero. But an induced current still appears. We must conclude that there is an induced electric field that causes the current to flow.

## Example

A conducting loop is moving in a spatially uniformmagnetic field. 
\input{EMF and Induced Fields/figures/Moving_Loop}

1.  What is the direction of Lorentz force on the electrons in each segment of the wire?

2.  Based on the result of (1), do you expect a current to flow?

3.  Based on Lenz's law, do you expect a current to flow?

{\bf Answer}:

1.  Upwards on all sides. 

2.  The magnetic force will not cause the charges to rotate around the loop. 

3.  No current is expected because the magnetic flux through the loop is not changing.

## Problem

A conducting bar slides along a U-shaped conducting wire as shown in a region of space where an external magnetic field is spatially uniform.

\input{EMF and Induced Fields/figures/Slide_Wire}

1.  What is the direction of Lorentz force on the electrons in each segment of the wire?

    {\bf Answer}:

    The Lorentz force will be zero on all sides (because $\mathbf{v}=0$) except for the moving wire. On the moving wire, $\mathbf{v}\times \mathbf{B}_{ext}$ is downwards (with a small component to the left because the velocity in the Lorentz force equation contains the velocity of the charge as it moves along the wire). The force on an electron will be in the opposite direction. 

2.  Based on the result of (1), do you expect a current to flow?

    {\bf Answer}: Clockwise.

3.  Based on Lenz's law, do you expect a current to flow? If yes, (a) in what direction and (b) is this direction consistent with your answer to 2.?

    {\bf Answer}:

    Yes, the current is expected to flow clockwise. If the normal to the loop is out of the page, the magnetic flux through the loops is increasing; a clockwise current creates a negative magnetic flux.

## Problem

\begin{center}
    \includegraphics[]{EMF and Induced Fields/figures/emf_and_Induced_Fields_Fig3.png}
\end{center}


1.  A copper wire loop is placed in a uniform magnetic field as shown. Determine whether there would be a current through the wire of the loop in each case below. {\bf Explain your answer in terms of magnetic forces exerted on the charges in the wire of the loop.} Recall that the magnitude of field lines is proportional to their spacing.
    1.  The loop is stationary.

    {\bf Answer}:

    If the loop is stationary, there are no moving charges so there is no Lorentz force on the charges and hence no current is induced in the loop.

    2.  The loop is moving to the right.

    {\bf Answer}:

    $$
    {\bf F} = q{\bf v} \times {\bf B}
    $$

    Both $\mathbf{v}$ and $\mathbf{B}$ are in the $\xhat$ direction so 
$v\hat{\bf x} \times B\hat{\bf x} = 0$.So no force and thus no current. 

    3.  The loop is moving to the left.

    {\bf Answer}:

    $$
    {\bf F} = q{\bf v} \times {\bf B}
    $$

    Both $\mathbf{v}$ and $\mathbf{B}$ are in the $\hat{\bf x}$ direction so 

    $$
    v (-\hat{\bf x}) \times B\hat{\bf x} = vb(-\hat{\bf x} \times \hat{\bf x}) = 0
    $$

    So no force and thus no current. 

## Problem

\begin{center}
    \includegraphics[]{EMF and Induced Fields/figures/emf_and_Induced_Fields_Fig5.png}
\end{center}

1.  In the figure above, there is a current running through a long straight wire as shown. For each conducting loop A-D determine:

    1.  The direction (clockwise or counterclockwise or zero) for the current induced in each loop.

    {\bf Answer}:

    A. no current

    B. clockwise

    C. clockwise

    D. no current

    2.  The direction of the net force on the loop – explain your reasoning.

    {\bf Answer}:

    A. no force -- there is no movement in a direction that is perpendicular to the current in the long wire and so there is no change in magnetic flux.

    {\small (This problem statement is missing information required to answer the question for case B. and C. If the velocity of an object is not changing, there is not a net force. Here we are not told whether or not an external force is being supplied to keep the velocity constant. In the answers for B. and C., it is assumed that there is not an external force being supplied to keep the velocity constant.)}

    B. and C. There is a net upwards magnetic force.

    D. no force -- there is no movement in a direction that is perpendicular to the current in the long wire and so there is no change in magnetic flux.

## Problem


\begin{center}
    \includegraphics[]{EMF and Induced Fields/figures/emf_and_Induced_Fields_Fig4.png}
\end{center}

1.  A conducting wire loop is placed in the magnetic field of a solenoid as shown. Determine whether there would be a current through the wire of the loop in each case below. If so, give the direction of the current. {\bf Explain your answer in terms of the magnetic forces exerted on the charges in the wire.}

    1.  The loop is stationary.

        {\bf Answer}: No moving charges so no force and thus no Lorentz force to start a current.

    2.  The loop is moving to the right.

    {\bf Answer}: 

    Let the $+\xhat$ direction be to the right and the $+\yhat$ direction be upwards. At the top of the ring, {\bf v} is in the $+\xhat$ direction, {\bf B} is in mostly in the $+\xhat$ direction and there is also a $-\yhat$ component, i.e., $B(a\hat{\bf x} + b\hat{\bf y}$).

    $$
    {\bf F} = qv\hat{\bf x} \times B(a\hat{\bf x} + b\hat{\bf y)} = qvbB(-\hat{\bf z})
    $$

    Thus the magnetic force is into the page at the top of the ring an so the current will be into the page at that location. This corresponds to a clockwise current if viewed from a point on the $+x$-axis.

    3.  The loop is moving to the left.

        {\bf Answer}: The same as above except that {\bf v} is in the $-\hat{\bf x}$ direction so:

        $$
        {\bf F} = qv(-\hat{\bf x}) \times B(a\hat{\bf x} + b\hat{\bf y}) = qvbB\hat{\bf z}
        $$

    Therefore the current will be counterclockwise if viewed from the $+x$-axis. 

1.  For each case in your answer to question 1. where there is an induced current find:

    1.  The direction of the induced magnetic field at the center of the loop due to the induced current.

        {\bf Answer}: Moving to the right: $-\hat{\bf x}$; Moving to the left: $+\hat{\bf x}$

    2.  Whether the loop is attracted to or repelled from the solenoid.

        {\bf Answer}: Moving to the right: repelled (field opposite solenoid's field); Moving to the left: attracted (field along solenoids field)

    3.  Whether the force required to move the loop increases or decreases as the loop is moved.

        {\bf Answer}: Moving to the right: increases, the magnetic field is increasing; Moving to the left: decreases, the magnetic field is decreasing
