```mdextension
Title: Lenz's Law
```

# Introduction

## Magnetic Flux

A changing magnetic flux through a closed conducting loop _induces_ the flow of a current in the loop.

In this activity, we will deal with a conducting loop that has a current that is not driven by a battery -- it will be driven by a change in magnetic flux through the loop. This change will _induce_ a current, and this induced current will create what we will refer to as an _induced_ magnetic field.

The general equation for magnetic flux is:

$$
\Phi_B = \int \bfvec{B}\cdot d\bfvec{A}
$$

If the magnitude of the magnetic field is not changing and the angle between the magnetic field vector and the area vector does not change, then integration is not required, and we can write

$
\Phi_B = \bfvec{B}\bfcdot \bfvec{A}
$
or, equivalently, $\Phi_B = BA\cos\phi$, where $\phi$ is the angle between the area vector and $\bfvec{B}$.

There are three ways in which $\Phi_B$ can change:

1. The magnitude of $\bfvec{B}$ (that is, $B$) can change. To do this, a magnet can be moved closer or farther away from a conducting loop, a loop can be moved closer or farther away from a magnet, or the current in the loop that is generating the magnetic field can be changed. See Example 29.1 in the textbook for an example of the creation of a changing magnetic field with an electromagnet.

2. The area $A$ can change. To do this, the loop cross--section can be expanded or contracted, either by heating or cooling a wire or, more commonly, using a device called a slidewire generator (see Example 29.5 and 29.6).

3. The angle $\phi$ can change. To do this, a conducting loop can be rotated (see Example 29.3). Electric motors use changes in $\phi$ to convert mechanical energy to electrical energy.

In this activity, you will determine the direction of the induced current in a conducting loop due to a changing magnetic flux through its area using Lenz's law for cases 1. and 2.

%Although Lenz's law can be used for case 3., we generally use Faraday's law first and then ask if our answer is consistent with Lenz's law. This is covered in a separate activity. Additionally, Lenz's law can be used to determine the direction of force or torque required by an external agent to cause the change in flux through the loop. This is also covered in a separate activity.

Lenz's law follows from Faraday's law. In principle, Faraday's law, with careful attention paid to signs, can be used to determine the direction of induced current, in which case Lenz's law is not needed. In a similar way that using the right--hand rules to determine the general direction for force can be used to check your math on a cross--product, Lenz's Law provides a check on the direction of the induced current when using Faraday's law.

\newpage

## Field Due to Current Loop

Given a loop of current in a plane, one can determine the direction of the magnetic field near the center of loop created by the current using the current loop right--hand rule. Wrap your fingers around the loop in the direction of the current -- your thumb points in the direction of the magnetic field.

<img src="figures/Figure-28.12_Young_Freedman_14th_Edition.png" width="50%"/>

**Figure 28.12 of Young and Freedman 14th Edition**

## Lenz's Law

As described in the textbook,

{\bf Lenz’s Law:} The direction of any magnetic induction effect is such as to oppose the cause of the effect.

Here, we'll use a longer but more descriptive definition.

{\bf Lenz’s Law alternative}: When the external magnetic flux through a conducting loop changes, a current appears (is induced) in the loop. This induced current creates an induced magnetic field. The direction of the induced current is such that the induced magnetic field it creates attempts to keep the magnetic flux unchanged.

In the examples given, we will first find the direction of the induced magnetic field. Then, we will ask what direction of the induced current is consistent with this induced magnetic field.

\newpage

# $B$ Changing

## Example

A spatially uniform external magnetic field points out of the page, and its magnitude is increasing in time.

<img src="figures/Field_Out_Of_Page.svg"/>

1. What is the direction of an induced magnetic field in the gray region that will counteract the change in the magnetic flux?

2. What is the direction of induced current in the loop that is consistent with the induced magnetic field found in part 1?

{\bf Answer}:

To determine the direction of the induced magnetic field, we draw field lines through the area at $t=0$ and then a short time later. On the left--hand side of the following figure, field lines are shown pointing out of the page. A short time later, at $t=\Delta t$, $B_{\text{ext}}$ has increased, so we draw more field lines pointing out of the page.

The induced magnetic field is in the direction that opposes the change in magnetic flux, so the induced field must be into the page. (Note that the induced field will not exactly cancel the increase in flux; the magnitude of the induced field will depend on how much current is induced, which depends on the resistance of the wires.)

Finally, we ask what direction of induced current in the loop creates this direction of $B_{\text{ind}}$. Using the current loop right--hand rule, it is a clockwise current.

<img src="figures/Field_Out_Of_Page_B_Increasing.svg"/>

\newpage

## Problems

###

A spatially uniform external magnetic field points into the page, and its magnitude decreases in time.

<img src="figures/Field_In_To_Page.svg">

1. Draw representitive field lines at $t=0$ and $t=\Delta t$ as done in the example.

   \ifsolutions
   \else
   <img src="figures/Loop_Sketch.svg">
   \fi

2. What direction would an induced magnetic field have to be to oppose the change in the magnetic flux?

   \ifsolutions
   {\bf Answer}: Into the page.
   \else
   \vspace{2em}
   \fi

3. What is the direction of induced current in the loop that is consistent with the induced magnetic field found in part 2?

   \ifsolutions
   {\bf Answer}: Clockwise.
   \else
   \vspace{2em}
   \fi

###

A spatially uniform external magnetic field points into the page, and its magnitude is increasing in time.

<img src="figures/Field_In_To_Page.svg">

1. Draw representitive field lines at $t=0$ and $t=\Delta t$ as done in the example.

   \ifsolutions
   \else
   <img src="figures/Loop_Sketch.svg">
   \fi

2. What direction would an induced magnetic field have to be to oppose the change in the magnetic flux?

   \ifsolutions
   {\bf Answer}: Out of the page.
   \else
   \vspace{2em}
   \fi

3. What is the direction of induced current in the loop that is consistent with the induced magnetic field found in part 2?

   \ifsolutions
   {\bf Answer}: Counterclockwise.
   \else
   \vspace{2em}
   \fi

###

<img src="figures/Ring_and_Solenoid.png"/>

A conducting wire loop is placed in the magnetic field of a solenoid, as shown. Treat the magnetic field of the solenoid as the external magnetic field. Several representative magnetic field lines are shown.

For the following case, determine if an induced magnetic field will appear and, if so, its direction. Then, determine the direction of induced current, if any, in the wire loop.

1. The loop is stationary.

   \ifsolutions
   {\bf Answer}: a. No flux change, so no induced magnetic field. b. No current.
   \else
   a. Direction of induced magnetic field:

   b. Direction of current in loop:

   \fi

2. The loop is moving to the right.

   \ifsolutions
   {\bf Answer}: As the loop moves to the right, the magnetic field is larger (field lines are more closely spaced). a. To keep the flux the same, an induced magnetic field pointing to the left is needed. b. The current in the loop is such that the current on the white part of the ring is upwards.
   \else
   a. Direction of induced magnetic field:

   b. Direction of current in loop:
   \fi

3. The loop is moving to the left.

   \ifsolutions
   {\bf Answer}: As the loop moves to the left, the magnetic field is smaller (field lines are less closely spaced). a. To keep the flux the same, an induced magnetic field pointing to the right will appear in the cross--section of the loop. b. The current in the loop is such that the current on the white part of the ring is downwards.
   \else
   a. Direction of induced magnetic field:

   b. Direction of current in loop:
   \fi

###

<img src="figures/Loops_in_Wire_Field.svg"/>

In the figure above, there is a current $I$ running through a long straight wire as shown.

For conducting loops A--D that are moving with a velocity in the direction shown, determine if the current flow is zero, clockwise, or counterclockwise.

   \ifsolutions
   {\bf Answer}: The field is out of the page above the long straight wire. Below, it is into the page (See section 28.3 of the Textbook). The magnitude of $\bfvec{B}$ is larger near the wire.

   A. Induced field is into page. The current is clockwise.

   B. No current.

   C. No current.

   D. Induced field is into page. The current is clockwise.
   \else
   \fi

# $A$ Changing

## Example

A spatially uniform external magnetic field points out of the page and it is not changing with time.

The conducting loop is heated causing the gray cross--sectional area to increase with time.

<img src="figures/Field_Out_Of_Page.svg"/>

1. What direction would an induced magnetic field have to be to oppose the change in the magnetic flux?

2. What is the direction of induced current in the loop that is consistent with the induced magnetic field found in part 1?

\ifsolutions
{\bf Answer}:

<img src="figures/Field_Out_of_Page_A_Increasing.svg">

To determine the direction of the induced magnetic field, we draw field lines at $t=0$. A short time later, at $t=\Delta t$, the area of the loop has increased an more field lines that are pointing out of the page pass through the area. In order to keep the total flux through the loop as it was at $t=0$, we need the induced field to cancel the added field lines. As shown, this induced field must be into the page.

Finally, we ask what direction of induced current in the loop creates this direction of $B_{\text{ind}}$. Using the current loop right--hand rule, it is a clockwise current.

1. Into the page.

2. A clockwise current creates a magnetic field into the page.
\else
\fi

## 

An external magnetic field points into the page and it is not changing with time.

The conducting loop is cooled causing the gray cross--sectional area to decrease with time.

<img src="figures/Field_In_To_Page.svg"/>

1. Draw representitive field lines at $t=0$ and $t=\Delta t$ as done in the example.

   \ifsolutions
   \else
   <img src="figures/Loop_Sketch.svg">
   \fi

2. What direction would an induced magnetic field have to be to oppose the change in the magnetic flux through the loop?


3. What is the direction of induced current in the loop that is consistent with the induced magnetic field found in part 1?

   \ifsolutions
   {\bf Answer}:
   2. The induced magnetic field will be into the page.

   3. By the right--hand rule, a clockwise current creates a magnetic field directed into the page.
   \else
   \fi

##

A conducting bar slides along a U-shaped conducting wire, as shown in a region of space where an external magnetic field is spatially uniform. (This is known as a "slidewire generator").

<img src="figures/Slide_Wire.svg"/>

\ifsolutions
\else
\vspace{5em}
\fi

1. What direction would an induced magnetic field have to be to oppose the change in the magnetic flux?

   \ifsolutions
   {\bf Answer}: Into the page.
   \else
   \vspace{3em}
   \fi

2. What is the direction of induced current in the loop that is consistent with the induced magnetic field found in part 1?

   \ifsolutions
   {\bf Answer}: Clockwise.
   \else
   \vspace{3em}
   \fi