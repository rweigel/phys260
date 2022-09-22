```mdextension
Title: Electric Potential
```

# Electric Potential Energy Differences, $\Delta U$

Recall from mechanics that the symbol $U$ was used to represent potential energy. The potential energy of an object increases when you do a positive amount of work on it. For example, if you lift a mass from the floor, you increase its potential energy. In addition, recall that work done on an object {\it changes} its potential energy, and this change is represented by $\Delta U$.

Mathematically, the work done by a force $\mathbf{F}$ in moving an object from position $a$ to position $b$ is

$$
W_{a\rightarrow b}=\int_a^b \mathbf{F}\cdot d\mathbf{l}
$$

There are three cases:

1. If a force is always perpendicular to the direction of movement, the work due to that force is zero. For example, a block sliding horizontally has a gravitational force exerted on it, but the gravitational force is downward and so perpendicular to the direction of motion. Thus, gravity does no work.

2. When the force on an object does not change when it is moved a distance $L$ from $a$ to $b$ and the direction of force is always in the same direction as the direction of movement, then

    $$W_{a\rightarrow b}=\int_a^b \mathbf{F}\cdot d\mathbf{l}=(\pm)|\mathbf{F}|L$$

    where $L$ is positive; the $+$ sign is used for a force that is in the direction of movement and the $-$ sign is used for a force that is in the opposite direction of movement. For example, if you lift a mass $m$ upwards by a distance $L$, the force you exert is in the same direction of movement, so you do a work of $mgL$. The gravitational force on the mass is in the opposite direction of movement, so the work done by the gravitational force is $-mgL$. If instead you lower the mass downwards, your force is upwards and the direction of motion is downwards, so the work you do is now $-mgL$ and the work done by the gravitational force is $+mgL$.

3. When the direction of force relative to the direction of movement changes (so the dot product changes) and/or the magnitude of force changes. This is covered on [page 755 of the textbook](https://drive.google.com/file/d/1KO0ETw12uhGYdBMHExKIdR_eCUhHB7dw/view?usp=sharing_remove_).


One of the most common difficulties in calculating work and energy is getting the correct sign for the answer. The following two problems have questions that help you determine the correct sign of work and changes in potential energy.

In general, determine the direction an object would would move when released from rest. If the object moves or is moved in that direction, its potential energy will decrease. If the object moves or is moved in the opposite direction, its potential energy will increase.

* Potential energy increases when you do positive work. That is, when your force on the object is in the direction that you move the object. One way of determining if an object's potential is higher is if it has more potential to do something. A mass lifted upwards has more potential to crush something (when you release it). If you lower a mass, it will have less potential to crush something. 
* Potential energy increases when a conservative force does negative work. 

**Conservative Forces**

If $\mathbf{F}$ is a special kind of force, called a _conservative_ force, we do not need to perform integration to every time that we want to compute the work. For each conservative force, there is an equation for $U$ (called potential energy, or PE) such that one needs to only know $U$ at $b$ and $a$. In this case,

$$
W_{a\rightarrow b}^{
\text{cons}} \equiv -\Delta U = -(U_b-U_a)
$$

where they symbol $\equiv$ is used to indicate a definition.

In mechanics, you have encountered two conservative forces

1. A constant force (e.g., the force on a small mass near Earth's surface)
2. A force that varies according to $\rhat/r^2$ (e.g., the gravitational force between two objects separated by a large distance)

In E&M, we enounter these same two types of conservative forces.

**Example**

Near Earth, the gravitation field is nearly constant. If point $a$ is a point on the floor and point $b$ is a point $1\text{ m}$ above $a$, using

$$W_{a\rightarrow b}=(\pm)|\mathbf{F}|L$$

1. how much work is required by you to lift the object from $a$ to $b$?;
2. how much work is is done by the gravitational field?

The equation for $U$ for a mass $m$ in a constant gravitational field $g~$ is $mgy$. Use $W_{a\rightarrow b}^{\text{cons}} \equiv -\Delta U = -(U_b-U_a)$

3. to find the work done by the gravitational field when the object is moved from $a$ to $b$.

**Solution**

1. Your force on the object must be upwards in order to lift it upwards, so the force is in the direction of displacement. So $W_{a\rightarrow b}=(+)mgL$. (This is actually the minimum amount of work that you would need to do; if there is any type of friction, more work will be needed.)

 
2. Τhe gravitational force is downwards, so the force is in the direction of displacement. So $W_{a\rightarrow b}=(-)mgL$


3. $U_b=mgy_b$ and $U_a=mgy_a$. Using

    $$W_{a\rightarrow b}^{\text{cons}} \equiv -\Delta U = -(U_b-U_a)$$

    gives

    $W_{a\rightarrow b}^{\text{cons}} = (mgy_b-mgy_a) = -mg(y_b-y_a) = -mgL$, which matches the answer to 2., as expected.

## Problem -- Uniform Field

The following diagram shows a region of space where the electric field is constant and has a value of $3\text{ N/C}$.

<img src="figures/Uniform_Field.svg"/>

1.  You place a charge of $+3\text{ C}$ at point $A$. What happens to that charge when it is released?

    {\bf Answer}: Moves to right. By convention field lines point in direction of force on positive charge.

2.  You move charge of $+3\text{ C}$ from $a$ to $b$. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the charge changed?

    {\bf Answer}: The charge naturally wants to move from A to B since it is a positive charge and the field line direction indicates the direction of force on a postive charge. The force the field exerts on the charge is $\mathbf{F}=Q\mathbf{E}=(3\text{ C})(3\text { N/C})\ihat = (9\text{ N})\ihat$, where $\ihat$ points to the right. Your force is equal and opposite. The work done by you is the force over the path parallel to the field: 

    $$
    W_{a\rightarrow b}=\int_a^b \mathbf{F}\cdot d\mathbf{l}=(\pm)|\mathbf{F}|L
    $$ 

    So your work is $(-9\text{ N})(2\text{ m}) = -18 \text{ J}$.

    (a) $(-9 \text{ N})(2\text {m})=-18\text{ J}$, (b) $(+9 \text{ N})(2\text {m})=+18\text{ J}$, (c) $\Delta U = -18\text{ J}$ The change in PE is equal and opposite to the work done by the field.

3.  You place a charge of $-3\text{ C}$ at point $a$. What happens to that charge when it is released?

    {\bf Answer}: Moves to left.

4.  A charge of $-3\text{ C}$ is moved from $a$ to $b$. How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the charge changed?

    {\bf Answer}: (a) $+18\text{ J}$, (b) $-18\text{ J}$, (c) $\Delta U = +18\text{ J}$ The change in PE is equal and opposite to the work done by the field.

5.  You move a charge of $+3\text{ C}$ straight downward from $a$ to $c$. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the charge changed?

    {\bf Answer}: Your force and the force due to the field are both perpendicular to the direction of movement. So the work done by both forces is zero: (a) $0\text{ J}$ (b) $0\text{ J}$ (c) $0 \text{ J}$.

6.  If you move a charge of $-3\text{ C}$ from $a$ to $c$ but deviate from a straight line, will your answers to the previous problem change? If no, explain why. If yes, provide new answers.

    {\bf Answer}: No, they won't change. Think of movement along a smooth and curved line as being made of a series of tiny equal-sized steps in the vertical and horizontal directions. There is no work associated with the vertical steps. There is positive work associated with steps to the right and negative work associated with steps to the left. To get from $A$ to $C$ along an arbitrary path, you must take an equal number of steps to the left as you do to the right. See also Figure 23.1 and 23.2 which describe how the work done by a conservative force does not depend on path.

## Problem -- Radial Field

In the previous problem, a charge was moved in a region of space where the electric field was constant and so the calculation of work did not require integration. In this problem, the electric field is not constant and so integration is required. The type of integration that must be performed to compute work in this case is given by [Equation 23.8 in the textbook](https://drive.google.com/file/d/1KO0ETw12uhGYdBMHExKIdR_eCUhHB7dw/view?usp=sharing_remove_).

<img src="figures/Radially_Inward_Field.svg"/>

There is a charge of $-6\text{ C}$ at the origin. Some electric field lines for this charge are shown. To simplify the math, use $k=9\cdot 10^9\text{ N}\cdot \text{m}^2/\text{C}^2$.

1.  You move a charge of $+3\text{ C}$ from $a$ to $b$. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the moved charge changed?

    {\bf Answer}: According to equation 23.8, the work done by the field, labeled $W^E$ here, when a charge $q_0$ is moved from a distance $r_a$ to a distance $r_b$ from a charge $q$ is

    $$
    W^E_{a\rightarrow b} = kqq_o\left(\frac{1}{r_a}-\frac{1}{r_b}\right)
    $$

    For this problem, $q=-6\text{ C}$, $q_0=3\text{ C}$, $r_a=3\text{ m}$, and $r_b=2\text{ m}$.

    $$
    W^E_{a\rightarrow b} = (9\cdot 10^9)(-6)(+3)\left(\frac{1}{3}-\frac{1}{2}\right)\text{ J} = +27\cdot 10^9\text{ J}
    $$

    This is the answer for (b). Note that the work is positive as expected -- the force on the charge is in the same direction as its movement. The work that you do is equal and opposite to the work that the field does. The change in potential is equal and opposite to the work done by the field. In summary, (a) $-27\cdot 10^9\text{ J}$, (b) $+27\cdot 10^9\text{ J}$, (c) $-27\cdot 10^9\text{ J}$. (Use the techniques given in the previous problem to make sure that the signs of these answers are correct.) Note that the answer of $27\cdot 10^9\text{ J}$ is unphysically large; it is the amount of energy that you would need to lift $27\cdot 10^9\text{ kg}$ (about $5$ million elephants) by $1\text{ m}$. 

2.  You move a charge of $-3\text{ C}$ from $a$ to $b$. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the moved charge changed?

    {\bf Answer}: (a) $+27\cdot 10^9\text{ J}$, (b) $-27\cdot 10^9\text{ J}$, (c) $+27\cdot 10^9\text{ J}$. 

3.  You move a charge of $-3\text{ C}$ from $b$ to $c$ along the dotted line. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the moved charge changed?

    {\bf Answer}: (a) $0\text{ J}$, (b) $0\text{ J}$, (c) $0\text{ J}$

4. You move a charge of $-3\text{ C}$ from $c$ to $b$ but deviate from the dotted line. (a) How much work did you do? (b) How much work was done by the electric field? (c) By how much has the potential energy of the moved charge changed?

    {\bf Answer}: (a) $0\text{ J}$, (b) $0\text{ J}$, (c) $0\text{ J}$

# Electric potential difference, $\Delta V$

In the previous section, we considered moving an arbitrary amount of charge (either positive or negative) from point $a$ to point $b$ and computed its change in potential energy $\Delta U$. 

An electric potential difference $\Delta V$ is defined to be the change in electric potential energy of a (positive by convention) test charge when it is moved from point $a$ to point $b$ divided by the charge on the test charge.

As a result, the only difference between the $\Delta U$ calculations performed previously and $\Delta V$ calculations is that we first compute $\Delta U$ for a $+1\text{ C}$ charge. To get $\Delta V$, we simply divide by $\Delta U$ by $+1\text{ C}$.

The definition of electric potential is similar to the definition of electric field in that they both involve consideration of a test charge. That is, the electric field is the force on a test charge divided by the magnitude of the test charge:

$$\mathbf{E} = {\mathbf{F}}/{q_o}$$

A change in potential is the change in potential of a  test charge divided by the magnitude of the test charge's charge:

$$\Delta V = {\Delta U}/{q_o}$$

The advantage of using changes in electric potential ($\Delta V$) as opposed to changes in electric potential energy ($\Delta U$) of a specific amount of charge is that once the electric potential difference $\Delta V$ is known for a test charge, the change in potential energy for an arbitrary amount of charge $Q$ can be computed by simply multiplying $\Delta V$ and $Q$. This is similar to the advantage of the electric field. If we know the electric field at a given point, we can find the force on an arbitrary charge $Q$ by multiplying $\mathbf{E}$ and $Q$.

## Problem

The following diagram shows a region of space where the electric field is constant and has a value of $3$~N/C. 

<img src="figures/Uniform_Field.svg"/>

1. What is difference in electric potential $\Delta V = V_B-V_A$.

    {\bf Answer}: As discussed in the introduction to this section, the difference in electric potential can be determined by first computing $\Delta U$ for a $+1\text{ C}$ charge. Then $\Delta V = \Delta U/(1\text{ C})$. The steps for computing $\Delta V$ for a $+1\text{ C}$ charge will be identical to those in problem 1.1.2 of this tutorial. The result is $\Delta U=-6\text{ J}$. Thus

    $$\Delta V = \frac{-6\text{ J}}{+1\text{ C}}= -6\text{ Volt}$$

    A faster way of solving this is to simply compute $\Delta V$ by using $\Delta U$ for the $3\text{ C}$ charge and dividing by $3\text{ C}$. This is also valid and makes sense -- a difference in potential from point $A$ to point $b$ corresponds to the change in potential energy associated with moving a positive unit of charge from point $A$ to point $b$. If you computed the change in energy associated with moving with 3 units of charge, then you divide this energy by 3 to get the difference in potential.

2. What is the difference in electric potential $\Delta V = V_B-V_C$.

    {\bf Answer}: $-6\text{ Volts}$. This is the same as $(V_B - V_A) + (V_A$ - $V_C) = -6\text{ Volts} + 0 = -6\text{ Volts}$

3. You move a charge of $+3\text{ C}$ from $a$ to $b$. By how much has the electric potential energy of the moved charge changed?

    {\bf Answer}: This question was already answered in problem 1.1.2. But given $\Delta V$, we can compute $\Delta U$:

    $$\Delta U = Q\Delta V=(3\text{ C})(-6\text{ Volt})=(3\text{ C})\left(-6\frac{\text{ J}}{ \text{ C}}\right)=-18\text{ J}$$

4. You move a charge of $-3\text{ C}$ from $a$ to $b$. By how much has the electric potential energy of the moved charge changed?

    {\bf Answer}: This question was already answered in problem 1.1.2. But given $\Delta V$, we can compute $\Delta U$:

    $$
    \Delta U = Q\Delta V=(-3\text{ C})(-6\text{ Volt})=(-3\text{ C})\left(-6\frac{\text{ J}}{ \text{ C}}\right)=+18\text{ J}
    $$

4.  You move a charge of $-3\text{ C}$ from $b$ to $c$. By how much has the electric potential energy of the moved charge changed?

    {\bf Answer}: The move from $b$ to $c$ can be made by a move from $b$ to $a$ then a move from $a$ to $b$. The change in potential in going from $b$ to $a$ is opposite the change in potential in going from $a$ to $b$, which was found to be $-6\text{ Volts}$. The change in potential in going from $a$ to $c$. Thus

    $$
    \Delta U = Q\Delta V=(-3\text{ C})(+6\text{ Volt})=-18\text{ J}
    $$

## Problem

<img src="figures/Radially_Inward_Field.svg"/>

There is a charge of $-6\text{ C}$ at the origin. Some electric field lines for this charge are shown. To simplify the math, use $k=9\cdot 10^9\text{ N}\cdot\text{m}^2/\text{C}^2$.

1.  What is difference in potential $\Delta V = V_b-V_a$?

    {\bf Answer}:

    In general, the potential at a point in space due to a point charge a distance $r$ from that point is $V={kq}/{r}$.

    $$V_A=\frac{k(-6\text{ C})}{3\text { m}}=-18\cdot 10^9\text{ Volt}$$

    $$V_B=\frac{k(-6\text{ C})}{2\text { m}}=-27\cdot 10^9\text{ Volt}$$

    $$V_B-V_A=-9\cdot 10^9\text{ Volt}$$

    A negative value is expected because a positive charge placed at $a$ will tend to move towards $b$, which has a lower potential.

2.  What is difference in electric potential $\Delta V = V_c-V_a$.

    {\bf Answer}: The potential at $b$ is the same as the potential at $c$. This can be seen mathematically from the equation $V=\frac{kq}{r}$ -- at $A$ and $b$, $r$ is the same. Physically, in moving from $A$ to $b$ along the dotted line, no work is required because the electric field is perpendicular to this path. The problem statement did not require moving from $a$ to $c$ along the dotted line, but was established earlier, the changes in potential energy are independent of path for a conservative force, so we are free to choose a convenient path. Based on this, $V_c-V_a=V_b-V_a$ and so the answer is the same as the previous problem.

3.  You move a charge of $-3\text{ C}$ from $a$ to $b$. By how much has the electric potential energy of the moved charge changed?

    {\bf Answer}:

    This is most easily found using

    $$\Delta U = U_{final}-U_{initial}= Q{\Delta V}=Q(V_{final}-V_{initial})$$

    Earlier it was found $V_B-V_A=-9\cdot 10^9\text{ Volt}$. As a result, 

    $$U_B-U_A= (-3\text{ C})(V_B-V_A)=+27\cdot 10^9$$

    This answer matches the answer for an identical question in problem 2.1.2 of this tutorial.

4.  You move a charge of $-3\text{ C}$ from $b$ to $c$. By how much has the electric potential energy of the moved charge changed?

    {\bf Answer}: $0\text{ J}$. See answer to question 1. for the justification.

# $\Delta U$ and $\Delta V$ and Superposition

The electric potential energy of a charge $q_0$ that is a distance of $r_1$ from a charge $q_1$ is defined to be 

$$
U=k\frac{q_0q_1}{r_1}
$$

In this formula, if the charges have opposite signs then $U$ is negative; if they have the same sign then $U$  is positive. Note that there is a sign associated with the potential energy but the direction of the vector that connects the charges does not matter; the equation for $U$ only involves the values of the charges and the magnitude of the separation distance between them.

Consider next the potential energy of charge $q_0$ when it is a distance $r_1$ from charge $q_1$ and a distance $r_2$ from charge $q_2$. Because potential energy is a scalar and not a vector, the potential energy of $q_0$ is the {\bf algebraic} sum, rather than the vector sum, of the potential energies due to $q_1$ and $q_2$

$$
U=k\frac{q_0q_1}{r_1}+k\frac{q_0q_2}{r_2}
$$

More generally, if there is a group of $N$ charges, the potential energy of charge $q_0$ is

$$
U=k q_0 \sum_{i=1}^N {\frac{q_i}{r_i}}
$$

Similarly, the electric potential at a point in space due to a group of $N$ charges is the {\bf algebraic} sum of the potentials due to each of the charges at that point in space

$$
V=k \sum_{i=1}^N {\frac{q_i}{r_i}}
$$

## Problem

<img src="figures/Collection_of_Charges.svg"/>

1. What is the potential energy of the charge $q_0$ in the diagram shown? 

    {\bf Answer}

    $$
    U = \frac{kq_oq_1}{r_1}+\frac{kq_oq_2}{r_2}+\frac{kq_oq_3}{r_3}
    $$

    This represents that amount of energy it would take to move charge $q_o$ from infinity to its position on the diagram.

2. What is the potential at the position of $q_0$ if that charge were to be removed (i.e., the potential due to charges $q_1$, $q_2$, and $q_3$)? 

    {\bf Answer} From $U=QV$, where here $Q=q_o$, $V=U/q_o$ 

    $$
    V = \frac{kq_1}{r_1}+\frac{kq_2}{r_2}+\frac{kq_3}{r_3}
    $$

    That is, the potential at a given location is found from potential energy of a charge at that location by dividing by the charge's potential energy by the value of the charge. 

3. Can you find the potential energy at the position of $q_0$ if that charge were to be removed? Why or why not? 

    {\bf Answer}: No. It does not make sense to ask what the potential energy is at a point in space. Only physical objects (e.g., masses, charges) have potential energy.

4. Explain the difference between potential and potential energy. 

    {\bf Answer}: A potential is a value associated with a location in space and an electric potential is created by charges at all locations in space.

    Potential energy is the energy associated with an object at a given location in space. The electric potential energy of a charge is the energy required to move it from a large distance away from all other charges to a given location in space. The electric potential energy of a charge $Q$ at a point in space is related to the electric potential at that point in space by $U=QV$.

## Problem

Given a point charge $q_1$ at the origin:

1. Write the general equation for the potential of a charge $q$.

2. Find the electric potential, $V$, at $(x,y) = (d,0)$.

3. If a charge $q_2$ is placed at $(x,y) = (d,0)$, find the electric potential, $V$, at $(x,y) = (-d,0)$ (hint - it is the sum of the potentials due to $q_1$ and $q_2$).

4. How much work is required to place $q_3$ at $(x,y) = (-d,0)$? Note that the work required is also referred to as the potential energy, $U$, of $q_3$.

In summary, to find the work required to put a charge $Q$ at point $P$ (or, equivalently, the electric potential energy $U$ of a single charge $Q$ when it is at point $P$), find the potential $V$ at point $P$ due to all of the other charges and then $U = QV$.

# Work Required to Assemble a System of Charges

In the previous problem you computed the work required to move $q_3$ to $(x,y) = (-d,0)$ after $q_2$ was in place. The total work required to assemble the system of three charges is larger than this work because it also took work to move $q_2$ into place. Given a point charge $q_1$ at origin, as in the previous question:

1. how much work is required to move $q_2$ to $(x,y) = (d,0)$?;

2. how much work is required to move $q_3$ to $(x,y) = (-d,0)$ if only $q_1$ is present?;

3. how much work is required to move $q_3$ to $(x,y) = (-d,0)$ if only $q_2$ is present?

4. The total work required to assemble the system of three charges is the sum of the work from parts a., b., and c. Write the equation for this sum. This sum is known as the total potential energy of the system of charges.