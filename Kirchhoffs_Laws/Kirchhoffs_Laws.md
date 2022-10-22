```mdextension
Title: Kirchoff's Circuit Laws
```

# Introduction

To find the current through each resistor in a circuit with only batteries and resistors, Kirchhoff’s Current Law and Kirchhoff’s Voltage Rule can be used.

1. Kirchhoff’s Voltage Law (KVL): The sum of all voltage changes around a closed loop must equal zero.
2. Kirchhoff’s Current Law (KCL): The sum of all currents entering and exiting a junction must equal zero.

**General procedure**

1. Assume directions of current.
2. Write equations for KCL for nodes.
3. Write equations for KVL for loops using the assumed direction of current.
4. Solve for currents.

**Sign conventions**

If you get a negative number for a current, your assumed direction was wrong.

When you write KVL, you must choose a direction that you move around the loop. If you "step" across a resistor $R$ in the direction of an assumed current $i$, the voltage change is $-iR$. If you "step" across in the direction opposite of $i$, the voltage change is $iR$.

If you step across a battery with emf $\mathcal{E}$ from the $-$ to the $+$, the voltage change is $+\mathcal{E}$. If you step across a battery with emf $\mathcal{E}$ from the $+$ to the $-$, the voltage change is $-\mathcal{E}$. _The direction of the assumed current does not matter._

\newpage

# Single Loop Circuit

In a single loop circuit, only KVL is needed to find the current.

<img src="figures/Single_Loop.svg">

1. Assume the direction of current $I$ in the above circuit is counterclockwise. Write the equation for KVL and then solve for $I$.

2. Assume the direction of current $I$ in the following circuit is clockwise. Write the equation for KVL and then solve for $I$.

3. Which value for $I$ found above is correct?

4. If you removed the bottom resistor and replaced the top resistor with a resistor with resistance $2R$, would $I$ change?

# Multiple Loop Circuit I

Assume the direction of currents $I_1$, $I_2$, and $I_3$ in the following circuit are as shown.

<img src="figures/Multiple_Loops_I.svg">

1. Write the equation for KVL for loop A.

2. Write the equation for KVL for loop B. 

3. Write the equation for KCL for node X.

Use the three equations found above to solve for the three unknowns, $I_1$, $I_2$, and $I_3$.

\newpage

# Multiple Loop Circuit II

In the circuit for the previous problem, there are three possible loops. The third loop is loop C. indicated below.

<img src="figures/Multiple_Loops_II.svg">

1. Write the equation for KVL for loop C.

2. Use the equation for KVL for loop B. and the KCL equation for node X from the previous problem along with the KVL equation for loop C to find $I_1$, $I_2$, and $I_3$. (You should get the same answers.)

# Redundant Equations

When solving circuit problems with multiple loops, you will generally find that you can use KVL and KCL to write more equations than there are unknowns. If you encounter a situation where you wrote $N$ equations based on KVL and KCL but cannot find $N$ unknows, the reason is that two or more of the $N$ equations that you wrote were not independent. To demonstrate this, for the circuit below,

1.  Write the KCL equation for node X

2.  Write the KCL equation for node Y

3.  Write the KVL equation for loop A
 
4.  Attempt to use the above three equations to solve for $I_1$, $I_2$, and $I_3$.

