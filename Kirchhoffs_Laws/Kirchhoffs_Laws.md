```mdextension
Title: Kirchoff's Circuit Laws
```

# Introduction

To find the current through each resistor in a circuit with only batteries and resistors, Kirchhoff’s Current Law and Kirchhoff’s Voltage Rule can be used.

1. Kirchhoff’s Voltage Law (KVL): The sum of all voltage changes around a closed loop is zero. 
2. Kirchhoff’s Current Law (KCL): The sum of all currents entering and exiting a junction is zero. Or, equivalently, the current flowing into a junction is equal to the current flowing out of a junction.

**General procedure**

To find the values of currents in a circuit, 

1. assume directions of current,
2. write equations for KCL for junctions,
3. write equations for KVL for loops, and
4. solve for currents. If you get a negative value for a current, the actual direction of current flow is opposite to what you assumed in 1.

**Note on Equivalent Resistances**

You may have already had experience solving for currents in circuits using equivalent resistances. In this activity, do not use equivalent resistances unless asked. The motivation is that after solving for currents without using equivalent resistances, you will better understand their interpretation and derivation.

%**KCL Rules**

%At a junction (a point where two or more currents flow into or out of), 

%**KVL Rules**

%When you write KVL, you must choose a direction that you "step" around the loop. If you "step" across a resistor $R$ in the direction of an assumed current $I$, the voltage change is $-IR$. If you "step" across in the direction opposite of $I$, the voltage change is $+IR$.

%If you step across a battery with emf $\mathcal{E}$ from the $-$ to the $+$, the voltage change is $+\mathcal{E}$. If you step across a battery with emf $\mathcal{E}$ from the $+$ to the $-$, the voltage change is $-\mathcal{E}$. _The direction of the assumed current does not matter._

%**Sign conventions**

%If you get a negative number for a current, your assumed direction was wrong.

\newpage

# Single Loop

Only KVL is needed to find the current in a single-loop circuit.

1. The direction of the unknown current $I$ in the following circuit is assumed to be counterclockwise. Write the equation for KVL stepping around the loop in the counterclockwise direction; then solve for $I$ in terms of $\mathcal{E}$ and $R$.

   <img src="figures/Single_Loop_CCW.svg" height="130px">

   \ifsolutions
   **Answer:** $\mathcal{E}-IR-IR=0 \quad \Rightarrow \quad I=\mathcal{E}/2R$
   \fi

2. The direction of current $I$ in the following circuit was assumed to be clockwise. Write the equation for KVL stepping around the loop in the counterclockwise direction; then solve for $I$ in terms of $\mathcal{E}$ and $R$.

   <img src="figures/Single_Loop_CW.svg" height="130px">

   \ifsolutions
   **Answer:** $\mathcal{E}+IR+IR=0 \quad \Rightarrow \quad I=-\mathcal{E}/2R$
   \fi

3. Which value for $I$ found above is correct?

   \ifsolutions
   **Answer**: Both are correct. A negative clockwise current is equivalent to a clockwise flowing current.
   \else
   \vspace{3em}
   \fi

4. In part 1., a counterclockwise current was assumed and you stepped in the counterclockwise direction. If you stepped in the clockwise direction, would your answer for $I$ be different? 

   \ifsolutions
   **Answer**: Answer same. KVL is $-\mathcal{E}+IR+IR=0 \quad \Rightarrow \quad I=\mathcal{E}/2R$
   \else
   \vspace{3em}
   \fi

5. For the circuit considered above, if you removed the bottom resistor and replaced the top resistor with a resistor with resistance $2R$, the following circuit results. What is the current $I$ for this circuit?

   \ifsolutions
   **Answer**: $I=\mathcal{E}/2R$ in counterclockwise direction.
   \else
   <img src="figures/Single_Loop_Equiv.svg" height="130px">
   \fi

\newpage

# Multiple Loops I

Assume the direction of currents $I_1$, $I_2$, and $I_3$ in the following circuit are as shown.

<img src="figures/Multiple_Loops_I.svg">

1. Write the equation for KVL for loop A.

   \ifsolutions
   **Answer**: $+\mathcal{E}-I_1R-I_3R=0$
   \else
   \vspace{3em}
   \fi

2. Write the equation for KVL for loop B.

   \ifsolutions
   **Answer**: $I_3R-I_2R=0$
   \else
   \vspace{3em}
   \fi

3. Write the equation for KCL for node X.

   \ifsolutions
   **Answer**: $I_3+I_2=I_1$
   \else
   \vspace{3em}
   \fi

4. Use the three equations found above to solve for the three unknowns, $I_1$, $I_2$, and $I_3$ in terms of $\mathcal{E}$ and $R$.

   \ifsolutions
   **Answer**:

   Eqn 1: $+\mathcal{E}-I_1R-I_3R=0$

   Eqn 2: $I_3R-I_2R=0$

   Eqn 3: $I_3+I_2=I_1$

   From Eqn 2., $I_2=I_3$ (this is expected, why?). Sub this into Eqn. 3 to get $I_3=I_1/2$. Plug this into Eqn 1. to get $I_1=(2/3)(\mathcal{E}/R)$. Additional substitution gives $I_2=I_3=(1/3)(\mathcal{E}/R)$.

   \else
   \vspace{6em}
   \fi

5. Check your answers by plugging your values for $I_1$, $I_2$, and $I_3$ into the equations that you wrote for parts 1.-3.

   \ifsolutions
   \else
   \vspace{3em}
   \fi

\newpage

# Multiple Loops II

In the circuit for the previous problem, there are three possible loops. The third loop is loop C. indicated below.

<img src="figures/Multiple_Loops_II.svg">

1. Write the equation for KVL for loop C.

   \ifsolutions
   **Answer**: $\mathcal{E}-I_1R-I_2R=0$
   \else
   \vspace{3em}
   \fi

2. Use the equation for KVL for loop B. and the KCL equation for node X from the previous problem along with the KVL equation for loop C to find $I_1$, $I_2$, and $I_3$ in terms of $\mathcal{E}$ and $R$. (You should get the same answers.)

\newpage

# Redundant Equations

When solving circuit problems with multiple loops, you will generally find that you can use KVL and KCL to write more equations than there are unknowns. If you encounter a situation where you wrote $N$ equations based on KVL and KCL but cannot find $N$ unknowns, the reason is that two or more of the $N$ equations that you wrote were not independent. To demonstrate this, for the following circuit,

<img src="figures/Multiple_Loops_III.svg">

1. write the KCL equation for node X,

   \ifsolutions
   \else
   \vspace{3em}
   \fi

2. write the KCL equation for node Y,

   \ifsolutions
   \else
   \vspace{3em}
   \fi

3. write the KVL equation for loop A, and

   \ifsolutions
   \else
   \vspace{3em}
   \fi
 
4. attempt to use the above three equations to solve for $I_1$, $I_2$, and $I_3$ in terms of $\mathcal{E}$ and $R$.

\newpage

# Using Equivalent Resistances

The analysis of the circuit considered previously could have been simplified if we had combined the lower two resistors into an equivalent resistor. In this case, we can easily solve for $I_1$ using the equivalent circuit in the middle.

<img src="figures/Multiple_Loops_IV.svg">

1. For the middle circuit, find $I_1$ in terms of $\mathcal{E}$ and $R$.

   \ifsolutions
   \else
   \vspace{3em}
   \fi

2. Use KVL for loop B and $I_1=I_2+I_3$ to find $I_2$ and $I_3$ in terms of $\mathcal{E}$ and $R$.

   \ifsolutions
   \else
   \vspace{3em}
   \fi

An alternative to the last step is to recognize that the voltage drop across both of the bottom two resistors is $V = I_1R/2$. Then the current through both resistors is $I_2=I_3=V/R$. Use this equation to check your answer to 2.

\ifsolutions
\else
\vspace{2em}
\fi

# Using Equivalent Resistances

Find the current through all resistors in the following circuit in terms of $\mathcal{E}$ and $R$.

<img src="figures/Multiple_Loops_V.svg">
