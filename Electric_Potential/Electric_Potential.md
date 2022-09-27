```mdextension
Title: Electric Potential
```

# Electric Potential Energy Differences, $\Delta U$

Recall from mechanics that the symbol $U$ was used to represent potential energy. The potential energy of an object increases when you do a positive amount of work on it. For example, if you lift a mass from the floor, you increase its potential energy. In addition, recall that work done on an object {\it changes} its potential energy, and this change is represented by $\Delta U$.

Mathematically, the work done by a force $\bfvec{F}$ in moving an object from position $a$ to position $b$ is

$$
W_{a\rightarrow b}=\int_a^b \bfvec{F}\bfcdot d\bfvec{l}
$$

Another way of writing $\bfvec{F}\bfcdot d\bfvec{l}$ is $|F|dl\cos\phi$, where $\phi$ is the angle between $\bfvec{F}$ and $d{\bfvec l}$.

There are three cases:

1. If a force is always perpendicular to the direction of movement, the work due to that force is zero. For example, a block sliding horizontally has a gravitational force exerted on it, but the gravitational force is downward and so is perpendicular to the direction of motion. Thus, gravity does no work.


2. When the force on an object does not change when it is moved a distance $L$ from $a$ to $b$ and the direction of force is always in the same direction as the direction of movement, then

   $$W_{a\rightarrow b}=\int_a^b \bfvec{F}\cdot d\bfvec{l}=(\pm)|\bfvec{F}|L$$

   where $L$ is positive; the $+$ sign is used for a force that is in the direction of movement, and the $-$ sign is used for a force that is in the opposite direction of movement. For example, if you lift a mass $m$ upwards by a distance $L$, the force you exert is in the same direction of movement, so you do a work of $mgL$. The gravitational force on the mass is in the opposite direction of movement, so the work done by the gravitational force is $-mgL$. If, instead, you lower the mass, your force is upwards, and the direction of motion is downwards, so the work you do is now $-mgL$, and the work done by the gravitational force is $+mgL$.


3. When the direction of force relative to the direction of movement changes (so the dot product changes) and/or the magnitude of force changes. This is covered on [page 755 of the textbook](https://drive.google.com/file/d/1KO0ETw12uhGYdBMHExKIdR_eCUhHB7dw/view?usp=sharing_remove_).


One of the most common difficulties in calculating work and change in potential energy is getting the correct sign for the answer. The following two problems have questions that help you determine the correct sign of work and changes in potential energy.

In general, determine the direction an object would move when released from rest (call this the "release direction"). If the object moves or is moved a small step in the release direction, its potential energy will decrease. If the object moves or is moved a small step in a direction opposite to the release direction, its potential energy will increase.

* The potential energy of an object increases when you do positive work on it. That is, when your force on the object is in the direction that you move the object. One way of determining if an object's potential is higher is if it has more potential to do something. A mass lifted upwards has more potential to crush something below it. If you lower a mass, it will have less potential to crush something.

* Potential energy increases when a conservative force (defined next) does negative work. 

**Conservative Forces**

If $\bfvec{F}$ is a special kind of force, called a _conservative_ force, we do not need to perform integration to every time that we want to compute the work. For each conservative force, there is an equation for $U$ (called potential energy, or PE) such that one needs to only know $U$ at $b$ and $a$. In this case,

$$
W_{a\rightarrow b}^{\text{cons}} \equiv -\Delta U = -(U_b-U_a)
$$

where they symbol $\equiv$ is used to indicate a definition.

In mechanics, you have encountered two conservative forces

1. A constant force (e.g., the force on a small mass near Earth's surface)
2. A force that varies according to $\rhat/r^2$ (e.g., the gravitational force between two objects separated by a large distance)

In E&M, we encounter these same two types of conservative forces.

**Example**

Near Earth, the gravitation field is nearly constant. If point $a$ is a point on the floor and point $b$ is a point $1\text{ m}$ above $a$, using

$$W_{a\rightarrow b}=(\pm)|\bfvec{F}|L$$

1. how much work is required by you to lift the object from $a$ to $b$?;
2. how much work is done by the gravitational field?

3. The equation for $U$ for a mass $m$ in a constant gravitational field $g~$ is $mgy$. Use $W_{a\rightarrow b}^{\text{cons}} \equiv -\Delta U = -(U_b-U_a)$ to find the work done by the gravitational field when the object is moved from $a$ to $b$.

**Solution**

1. Your force on the object must be upwards in order to lift it upwards, so your force is in the direction of movement. So $W_{a\rightarrow b}=(+)mgL$.
 
2. The gravitational force is downwards, so the force is opposite the direction of movement. So $W_{a\rightarrow b}=(-)mgL$


3. $U_b=mgy_b$ and $U_a=mgy_a$. Using

   $$W_{a\rightarrow b}^{\text{cons}} \equiv -\Delta U = -(U_b-U_a)$$

   gives

   $W_{a\rightarrow b}^{\text{cons}} = (mgy_b-mgy_a) = -mg(y_b-y_a) = -mgL$, which matches the answer to 2., as expected.

\newpage

## Problem -- Uniform Field

The following diagram shows a region of space where the electric field is constant and has a value of $3\text{ N/C}$.

<img src="figures/Uniform_Field.svg"/>

1. You place a charge of $+3\text{ C}$ at point $A$. What happens to that charge when it is released?

   \ifsolutions
   {\bf Answer}: Moves to right. By convention, electric field lines point in the direction of the force on a positive charge.
   \else
   <div style="height:3em"/>
   \fi

2. You move charge of $+3\text{ C}$ from $A$ to $B$. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the charge changed?

   \ifsolutions
   {\bf Answer}: The charge naturally wants to move from $A$ to $B$ since it is a positive charge and the field line direction indicates the direction of the force on a positive charge. The force the field exerts on the charge is $\bfvec{F}=Q\bfvec{E}=(3\text{ C})(3\text { N/C})\ihat = (9\text{ N})\ihat$, where $\ihat$ points to the right. Your force is equal and opposite. So your work is $(-9\text{ N})(2\text{ m}) = -18 \text{ J}$.

   (a) $(-9 \text{ N})(2\text { m})=-18\text{ J}$, (b) $(+9 \text{ N})(2\text { m})=+18\text{ J}$, and (c) $\Delta U = -18\text{ J}$ (the change in PE, $\Delta U$ is equal and opposite to the work done by the field).
   \else
   <div style="height:3em"/>
   \fi

3. You place a charge of $-3\text{ C}$ at point $A$. What happens to that charge when it is released?

   \ifsolutions
   {\bf Answer}: Moves to left.
   \else
   <div style="height:4em"/>
   \fi

4. A charge of $-3\text{ C}$ is moved from $A$ to $B$. How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the charge changed?

   \ifsolutions
   {\bf Answer}: (a) $+18\text{ J}$, (b) $-18\text{ J}$, and (c) $\Delta U = +18\text{ J}$ (the change in PE, $\Delta U$ is equal and opposite to the work done by the field).
   \else
   <div style="height:4em"/>
   \fi

5. You move a charge of $-3\text{ C}$ straight downward from $A$ to $D$. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the charge changed?

   \ifsolutions
   {\bf Answer}: Your force and the force due to the field are both perpendicular to the direction of movement. So the work done by both forces is zero: (a) $0\text{ J}$ (b) $0\text{ J}$ (c) $0 \text{ J}$.
   \else
   <div style="height:4em"/>
   \fi

6. If you move a charge of $-3\text{ C}$ from $A$ to $D$ but deviate from a straight line, will your answers to the previous problem change? If no, explain why. If yes, provide new answers.

   \ifsolutions
   {\bf Answer}: No, they won't change. Think of movement along a smooth and curved line as being made of a series of tiny and equal-sized steps in vertical and horizontal directions. There is no work associated with the vertical steps. There is positive work associated with steps to the right and negative work associated with steps to the left. To get from $A$ to $D$ along an arbitrary path, you must take an equal number of steps to the left and to the right. See also Figure 23.1 and 23.2 in the textbook, which describes how the work done by a conservative force does not depend on the path.
   \else
   <div style="height:3em"/>
   \fi

\newpage

## Problem -- Radial Field

In the previous problem, a charge was moved in a region of space where the electric field was constant and so the calculation of work did not require integration. In this problem, the electric field is not constant and so integration is required. The integration that must be performed to compute work in this case is given by [Equation 23.8 in the textbook](https://drive.google.com/file/d/1KO0ETw12uhGYdBMHExKIdR_eCUhHB7dw/view?usp=sharing_remove_).

<img src="figures/Radially_Inward_Field.svg"/>

There is a charge of $-6\text{ C}$ at the origin. Some electric field lines for this charge are shown. To simplify the calculations, use $k=9\cdot 10^9\text{ N}\cdot \text{m}^2/\text{C}^2$.

1. You move a charge of $+3\text{ C}$ from $A$ to $B$. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the moved charge changed?

   \ifsolutions
   {\bf Answer}: According to equation 23.8, the work done by the field, labeled $W^E$ here, when a charge $q_0$ is moved from a distance $r_a$ to a distance $r_b$ from a charge $q$ is

   $$
   W^E_{a\rightarrow b} = kqq_o\left(\frac{1}{r_a}-\frac{1}{r_b}\right)
   $$

   For this problem, $q=-6\text{ C}$, $q_0=3\text{ C}$, $r_a=3\text{ m}$, and $r_b=2\text{ m}$.

   $$
   W^E_{a\rightarrow b} = (9\cdot 10^9)(-6)(+3)\left(\frac{1}{3}-\frac{1}{2}\right)\text{ J} = +27\cdot 10^9\text{ J}
   $$

   This is the answer for (b). Note that the work is positive as expected -- the force of the electric field on the charge is in the same direction as its movement. The work that you do is equal to and opposite of the work that the field does. The change in potential is equal to and opposite of the work done by the field. In summary, (a) $-27\cdot 10^9\text{ J}$, (b) $+27\cdot 10^9\text{ J}$, (c) $-27\cdot 10^9\text{ J}$. Note that the answer of $27\cdot 10^9\text{ J}$ is unphysically large; it is the amount of energy that you would need to lift $27\cdot 10^9\text{ kg}$ (about $5$ million elephants) by $1\text{ m}$. 
   \else
   <div style="height:4em"/>
   \fi
   
2. You move a charge of $-3\text{ C}$ from $A$ to $B$. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the moved charge changed?

   \ifsolutions
   {\bf Answer}: (a) $+27\cdot 10^9\text{ J}$, (b) $-27\cdot 10^9\text{ J}$, (c) $+27\cdot 10^9\text{ J}$. 
   \else
   <div style="height:4em"/>
   \fi

3. You move a charge of $-3\text{ C}$ from $B$ to $D$ along the dotted line. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the moved charge changed?

   \ifsolutions
   {\bf Answer}: (a) $0\text{ J}$, (b) $0\text{ J}$, (c) $0\text{ J}$
   \else
   <div style="height:4em"/>
   \fi

4. You move a charge of $-3\text{ C}$ from $D$ to $B$ but deviate from the dotted line. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the moved charge changed?

   \ifsolutions
   {\bf Answer}: (a) $0\text{ J}$, (b) $0\text{ J}$, (c) $0\text{ J}$
   \fi

\newpage

# Electric potential difference, $\Delta V$

In the previous section, we considered moving an arbitrary amount of charge (either positive or negative) from point $a$ to point $b$ and computed its change in potential energy $\Delta U$. 

An electric potential difference $\Delta V$ is defined to be the change in electric potential energy of a (positive by convention) test charge when it is moved from point $a$ to point $b$ divided by the charge on the test charge.

As a result, the only difference between the $\Delta U$ calculations performed previously and $\Delta V$ calculations is that we first compute $\Delta U$ for a $+1\text{ C}$ charge. To get $\Delta V$, we simply divide by $\Delta U$ by $+1\text{ C}$.

The definition of electric potential is similar to the definition of the electric field in that they both involve consideration of a test charge. That is, the electric field is the force on a test charge divided by the magnitude of the test charge:

$$\bfvec{E} = {\bfvec{F}}/{q_o}$$

A change in electric potential is the change in electric potential energy of a positive test charge divided by the magnitude of the test charge's charge:

$$\Delta V = {\Delta U}/{q_o}$$

The advantage of using changes in electric potential ($\Delta V$) as opposed to changes in electric potential energy ($\Delta U$) of a specific amount of charge is that once the electric potential difference $\Delta V$ between two points is known for a test charge, the change in potential energy for an arbitrary amount of charge $Q$ can be computed by simply multiplying $\Delta V$ and $Q$. This is similar to the advantage of the electric field. If we know the electric field at a given point, we can find the force on an arbitrary charge $Q$ at that point by multiplying $\bfvec{E}$ and $Q$.

\newpage

## Problem

The following diagram shows a region of space where the electric field is constant and has a value of $3$~N/C. 

<img src="figures/Uniform_Field.svg"/>

1. What is the difference in electric potential $\Delta V = V_B-V_A$.

   \ifsolutions
   {\bf Answer}: As discussed in the introduction to this section, the difference in electric potential can be determined by first computing $\Delta U$ for a $+1\text{ C}$ charge. Then $\Delta V = \Delta U/(1\text{ C})$. The steps for computing $\Delta V$ for a $+1\text{ C}$ charge will be identical to those in problem 1.1.2 of this tutorial. Using these steps, the result for this problem is $\Delta U=-6\text{ J}$. Thus,

   $$\Delta V = \frac{-6\text{ J}}{+1\text{ C}}= -6\text{ Volt}$$

   A faster way of solving this is to simply compute $\Delta V$ by using $\Delta U$ for the $3\text{ C}$ charge considered in 1.1.2 ($-18\text{ J}$) and dividing by $3\text{ C}$. This is also valid and makes sense -- a difference in potential from point $A$ to point $B$ corresponds to the change in potential energy associated with moving a positive unit of charge from point $A$ to point $B$. If you computed the change in energy associated with moving with 3 units of charge, then you divide this energy by $3\text{ C}$ to get the difference in potential.
   \else
   <div style="height:4em"/>
   \fi

2. You move a charge of $+3\text{ C}$ from $A$ to $B$. By how much has the electric potential energy of the moved charge changed?

   \ifsolutions
   {\bf Answer}: This question was already answered previously in 1.1.2. But given $\Delta V$, we can compute $\Delta U$:

   $$\Delta U = Q\Delta V=(3\text{ C})(-6\text{ Volt})=(3\text{ C})\left(-6\frac{\text{ J}}{ \text{ C}}\right)=-18\text{ J}$$
   \else
   <div style="height:4em"/>
   \fi

3. You move a charge of $-3\text{ C}$ from $A$ to $B$. By how much has the electric potential energy of the moved charge changed?

   \ifsolutions
   {\bf Answer}: This question was already answered previously in 1.1.4. But given $\Delta V$, we can compute $\Delta U$:

   $$
    \Delta U = Q\Delta V=(-3\text{ C})(-6\text{ Volt})=(-3\text{ C})\left(-6\frac{\text{ J}}{ \text{ C}}\right)=+18\text{ J}
   $$
   \else
   <div style="height:4em"/>
   \fi

4. You move a charge of $-3\text{ C}$ from $B$ to $D$. By how much has the electric potential energy of the moved charge changed?

   \ifsolutions
   {\bf Answer}: The move from $B$ to $D$ can be made by moving from $B$ to $A$ and then moving from $A$ to $D$. The change in potential when moving from $B$ to $A$ is opposite to the change in potential when moving from $A$ to $B$, which was found to be $-6\text{ Volts}$. The change in potential in going from $A$ to $D$ is zero. Thus,

   $$
    \Delta U = Q\Delta V=(-3\text{ C})(+6\text{ Volt})=-18\text{ J}
   $$
   \else
   <div style="height:4em"/>
   \fi

5. What is the difference in electric potential $\Delta V = V_B-V_D$.

   \ifsolutions
   {\bf Answer}: $-6\text{ Volts}$. This is the same as $(V_B - V_A) + (V_A - V_D) = -6\text{ Volts} + 0 = -6\text{ Volts}$
   \else
   <div style="height:4em"/>
   \fi

\newpage

## Problem

There is a charge of $-6\text{ C}$ at the origin. Some electric field lines for this charge are shown. To simplify the math, use $k=9\cdot 10^9\text{ N}\cdot\text{m}^2/\text{C}^2$.

<img src="figures/Radially_Inward_Field.svg"/>

1. What is the difference in potential $\Delta V = V_B-V_A$?

   \ifsolutions
   {\bf Answer}:

   The potential at a point in space due to a point charge $q$ a distance $r$ from that point is $V={kq}/{r}$.

   $$V_A=\frac{k(-6\text{ C})}{3\text { m}}=-18\cdot 10^9\text{ Volt}$$

   $$V_B=\frac{k(-6\text{ C})}{2\text { m}}=-27\cdot 10^9\text{ Volt}$$

   $$V_B-V_A=-9\cdot 10^9\text{ Volt}$$

   A negative value is expected because a positive charge placed at $A$ will tend to move towards $B$, which has a lower potential.
   \else
   <div style="height:4em"/>
   \fi

2. You move a charge of $-3\text{ C}$ from $A$ to $B$. By how much has the electric potential energy of the moved charge changed?

   \ifsolutions
   
   {\bf Answer}:

   This is most easily found using

   $$\Delta U = Q{\Delta V}$$

   From part 1., $V_B-V_A=-9\cdot 10^9\text{ Volt}$. As a result, 

   $$U_B-U_A= (-3\text{ C})(V_B-V_A)=+27\cdot 10^9$$

  This answer matches the answer to the identical question of problem 1.1.2.
   \else
   <div style="height:4em"/>
   \fi

3. You move a charge of $-3\text{ C}$ from $B$ to $D$. By how much has the electric potential energy of the moved charge changed?

   \ifsolutions
   {\bf Answer}: $0\text{ J}$.
   \else
   <div style="height:4em"/>
   \fi

4. What is difference in electric potential $\Delta V = V_D-V_A$.

   \ifsolutions
   {\bf Answer}: The potential at $D$ is the same as the potential at $B$. This can be seen mathematically from the equation $V=\frac{kq}{r}$ -- at $D$ and $B$, $r$ is the same. Physically, in moving from $B$ to $D$ along the dotted line, no work is required because the electric field is perpendicular to this path. The problem statement did not require moving from $B$ to $D$ along the dotted line, but was established earlier, the changes in potential energy are independent of the path for a conservative force, so we are free to choose a convenient path. Based on this, $V_D-V_A=V_B-V_A$ and so the answer is the same as the previous problem.
   \else
   <div style="height:4em"/>
   \fi

\newpage

# $U$ and $V$ and Superposition

%Recall that the work done by the electric field when a charge $q_0$ is moved from $a$ to $b$ is

%$$
%W^E_{a\rightarrow b} = kqq_o\left(\frac{1}{r_a}-\frac{1}{r_b}\right)
%$$

%Plugging in $a=\infty$ and $b=r_1$ gives

%$$
%W^E_{\infty\rightarrow r_1}
%= kqq_o\left(\frac{1}{\infty}-\frac{1}{r_1}\right) 
%= -k\frac{q_0q_1}{r_1}
%$$

%$$
%W_{a\rightarrow b}^{
%\text{cons}} \equiv -\Delta U = -(U_b-U_a)
%$$

The electric potential energy of a charge $q_0$ that is a distance of $r_1$ from a charge $q_1$ is defined to be 

$$
U=k\frac{q_0q_1}{r_1}
$$

This corresponds to the work required to move $q_0$ from infinity to $r_1$. 
In this formula, if the charges have opposite signs then $U$ is negative; if they have the same sign then $U$  is positive. Note that there is a sign associated with the potential energy, but the direction of the vector that connects the charges does not matter; the equation for $U$ only involves the values of the charges and the magnitude of the separation distance between them. As a result, we can also state that the formula above corresponds to the work required to move $q_1$ from infinity to a distance $r_1$ from $q_0$.

Consider next the potential energy of charge $q_0$ when it is a distance $r_1$ from charge $q_1$ and a distance $r_2$ from charge $q_2$. Because potential energy is a scalar and not a vector, the potential energy of $q_0$ is the {\bf algebraic} sum, rather than the vector sum, of the potential energies due to $q_1$ and $q_2$

$$
U=k\frac{q_0q_1}{r_1}+k\frac{q_0q_2}{r_2}
$$

More generally, if there is a group of $N$ charges, the potential energy of charge $q_0$ is

$$
U=k q_0 \sum_{i=1}^N {\frac{q_i}{r_i}}
$$

Similarly, the electric potential at a point in space due to a group of $N$ charges is the {\bf algebraic} sum of the potentials due to each of the charges at that point in space:

$$
V=k \sum_{i=1}^N {\frac{q_i}{r_i}}
$$

\newpage

## Problem

<img src="figures/Collection_of_Charges.svg"/>

1. What is the potential energy of the charge $q_0$ in the diagram shown? 

   \ifsolutions
   {\bf Answer}

   $$
   U = \frac{kq_oq_1}{r_1}+\frac{kq_oq_2}{r_2}+\frac{kq_oq_3}{r_3}
   $$

   This represents the amount of energy it would take to move charge $q_o$ from infinity to its position on the 
   diagram.
   \else
   <div style="height:4em"/>
   \fi

2. What is the potential at the position of $q_0$ if that charge was not there (i.e., the potential due to charges $q_1$, $q_2$, and $q_3$)? 

   \ifsolutions
   {\bf Answer} From $U=QV$, where here $Q=q_o$, $V=U/q_o$ 
   $$
   V = \frac{kq_1}{r_1}+\frac{kq_2}{r_2}+\frac{kq_3}{r_3}
   $$

   That is, the potential at a given location is found from potential energy of a charge at that location by dividing by the charge's potential energy by the value of the charge.
   \else
   <div style="height:4em"/>
   \fi

3. Can you find the potential energy at the position of $q_0$ if that charge was not there? Why or why not? 

   \ifsolutions
   {\bf Answer}: No. It does not make sense to ask what the potential energy is at a point in space. Only physical objects (e.g., masses, charges) have potential energy.
   \else
   <div style="height:4em"/>
   \fi

4. Explain the difference between potential and potential energy. 

   \ifsolutions
   {\bf Answer}: Potential energy is the energy associated with an object at a given location in space. The electric potential energy of a charge is the energy required to move it from a large distance away from all other charges to a given location in space. The electric potential energy of a charge $Q$ at a point in space is related to the electric potential at that point in space by $U=QV$.
   \else
   <div style="height:4em"/>
   \fi

\newpage

## Problem

Given a point charge $q_1$ at the origin:

1. Write the general equation for the electric potential at a distance $r$ from $q_1$

   \ifsolutions
   $V=kq_1/r$
   \else
   <div style="height:3em"/>
   \fi

2. Find the electric potential, $V$, at $(x,y) = (-d,0)$ due to $q_1$.

   \ifsolutions
   $V_1(d,0)=kq_1/d$
   \else
   <div style="height:3em"/>
   \fi

3. If a charge $q_2$ is placed at $(x,y) = (d,0)$, find the electric potential, $V$, at $(x,y) = (-d,0)$ (hint -- it is the sum of the electric potentials at $(x,y)=(-d, 0)$ due to $q_1$ and $q_2$).

   \ifsolutions
   $V(-d,0)=V_1(-d,0)+V_2(-d,0) = kq_1/d + kq_2/2d$
   \else
   <div style="height:3em"/>
   \fi

4. How much work is required to place $q_3$ at $(x,y) = (-d,0)$?

   \ifsolutions
   $U=W=q_3V(-d,0)=q_3(kq_1/d + kq_2/2d)$
   \else
   <div style="height:3em"/>
   \fi

5. What is the potential energy, $U$, of $q_3$ when it is at $(x,y) = (-d,0)$?

   \ifsolutions
   See 4.
   \else
   <div style="height:3em"/>
   \fi

In summary, to find the work required to put a charge $Q$ at point $P$ (or, equivalently, the electric potential energy $U$ of a single charge $Q$ when it is at point $P$), find the potential $V$ at point $P$ due to all of the other charges and then $U = QV$.

\newpage

# Energy to Assemble a Collection of Charges

In the previous problem you computed the work required to move $q_3$ to $(x,y) = (-d,0)$ after $q_2$ was in place. The total work required to assemble the system of three charges is larger than this work because it also took work to move $q_2$ into place. Given a point charge $q_1$ at origin, as in the previous question,

1. how much work is required to move $q_2$ to $(x,y) = (d,0)$?;

   \ifsolutions
   $W = q_2V_1(0,d) = q_2(kq_1/d)$
   \else
   <div style="height:3em"/>
   \fi

2. how much work is required to move $q_3$ to $(x,y) = (-d,0)$ if only $q_1$ is present?;

   \ifsolutions
   $W = q_3V_1(-d,0) = q_3(kq_1/d)$
   \else
   <div style="height:3em"/>
   \fi

3. how much work is required to move $q_3$ to $(x,y) = (-d,0)$ if only $q_2$ is present?

   \ifsolutions
   $W=q_3V_2(-d,0)=q_3kq_2/2d$
   \else
   <div style="height:3em"/>
   \fi

4. The total work required to assemble the system of three charges is the sum of the work from parts 1.-3.. Write the equation for this sum in terms of the given variables. (This sum is known as the total potential energy of the system of charges -- see equation 23.11 of the textbook, which uses the same symbol $U$; ideally, they would have used $U_c$ to indicate that it applies to a collection of charges and not a single charge).

   \ifsolutions
   $W=q_2kq_1/d +  q_3(kq_1/d) + q_3kq_2/2d$
   \fi
