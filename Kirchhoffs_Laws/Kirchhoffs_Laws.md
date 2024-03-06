```mdextension
Title: Kirchhoff's Circuit Laws
```

# Introduction

To find the current through each resistor in a circuit with only resistors and batteries, Kirchhoff’s Current Law and Kirchhoff’s Voltage Law can be used.

1. Kirchhoff’s Current Law (KCL): The sum of all currents entering and exiting a junction is zero. Or, equivalently, the current flowing into a junction is equal to the current flowing out of a junction.
2. Kirchhoff’s Voltage Law (KVL): The sum of all voltage changes around a closed loop is zero. 

**General procedure**

To find the values of currents in a circuit, 

1. assume directions of current,
2. write equations for KCL for junctions,
3. write equations for KVL for loops, and
4. solve for currents. If you get a negative value for a current, the actual direction of current flow is opposite to what you assumed in 1.

To apply KVL, draw a closed loop and choose a direction to step around the loop. 

1. If stepping around the loop requires a step across a battery with emf $\mathcal{E}$ and the $-$ side is encountered first, the voltage change is $+\mathcal{E}$. If the $+$ side is encountered first, the voltage change is $-\mathcal{E}$. _The direction of current through the battery does not matter._

2. If stepping around the loop requires a step across a resistor $R$ and the direction of current $I$ through the resistor is the same as the step direction, the voltage change is $-IR$. If the current is opposite the step direction, the voltage change is $+IR$.

A common error is to assume every loop equation requires an emf.

**Note on Equivalent Resistances**

You may have already had experience solving for currents in circuits using equivalent resistances. In this activity, do not use equivalent resistances unless asked. The motivation is that you will better understand their interpretation and derivation after solving for currents without using equivalent resistances.

\ifsolutions
\else
\newpage
\fi

# Single Loop

Only KVL is needed to find the current in a single-loop circuit.

1. The direction of the unknown current $I$ in the following circuit is assumed to be counterclockwise. Write the equation for KVL by stepping around the loop counterclockwise; then solve for $I$ in terms of $\mathcal{E}$ and $R$.

   <img src="figures/Single_Loop_CCW.svg" height="130px">

   \ifsolutions
   **Answer:** $\mathcal{E}-IR-IR=0 \quad \Rightarrow \quad I=\mathcal{E}/2R$
   \fi

2. The direction of current $I$ in the following circuit was assumed to be clockwise. Write the equation for KVL stepping around the loop counterclockwise; then solve for $I$ in terms of $\mathcal{E}$ and $R$.

   <img src="figures/Single_Loop_CW.svg" height="130px">

   \ifsolutions
   **Answer:** $\mathcal{E}+IR+IR=0 \quad \Rightarrow \quad I=-\mathcal{E}/2R$
   \fi

3. Which value for $I$ found above is correct?

   \ifsolutions
   **Answer**: Both are correct and consistent. A negative current is equivalent to a positive current in the opposite direction. (You may recall from mechanics that when solving static equilibrium problems, you assume a direction for an unknown force $F$ on an object in a free-body diagram, sum all of the forces on it, and then solve for the unknown force. If the solution gives a negative $F$, you assumed the wrong direction for $F$.)
   \else
   \vspace{3em}
   \fi

4. In part 1., a counterclockwise current was assumed, and you stepped in the counterclockwise direction. If you stepped clockwise, would your answer for $I$ be different? 

   \ifsolutions
   **Answer**: Answer same. KVL is $-\mathcal{E}+IR+IR=0 \quad \Rightarrow \quad I=\mathcal{E}/2R$
   \else
   \vspace{3em}
   \fi

5. For the circuit in part 1., if you replace the bottom resistor with a wire and replace the top resistor with a resistor with resistance $2R$, the following circuit results. What is the current $I$ for this circuit?

   <img src="figures/Single_Loop_Equiv.svg" height="130px">

   \ifsolutions
   **Answer**: $I=\mathcal{E}/2R$ in counterclockwise direction. The fact that the answer here is the same as in 1. is related to the formula for the equivalent resistance of resistors in series: $R_{\text{eq}}=R_1+R_2$. Two resistors are in series if only one current path exists between them.
   \fi

\ifsolutions
\else
\newpage
\fi

# Multiple Loops I

<img src="figures/Parallel.svg" height="200px">

1. Use KCL at junction $X$ and KVL for loops $A$ and $B$ to show that $I_o=\mathcal{E}\left(\frac{1}{R_1}+\frac{1}{R_2}\right)$.

   \ifsolutions
   **Answer**:
   
   KVL for $A$: $+\mathcal{E}-I_1R_1=0\quad\Rightarrow\quad I_1=\mathcal{E}/R_1$

   KVL for $B$: $+I_1R_1-I_2R_2=0 \quad\Rightarrow\quad I_2 = I_1 R_1/R_2 = \mathcal{E}/R_2$

   KCL at $X$: $I_o=I_1+I_2 = \mathcal{E}/R_1 + \mathcal{E}/R_2 = \mathcal{E}\left(\frac{1}{R_1}+\frac{1}{R_2}\right)$
   \else
   \vspace{10em}
   \fi

2. If $R_2 > R_1$, which resistor will have more current?

   \ifsolutions
   **Answer**:
    
    $$\frac{I_2}{I_1} = \frac{R_1}{R_2} \quad \Rightarrow \quad I_2 < I_1$$ 
    
    One can also use the water flow analogy. If $R_2$ resists flow more than $R_1$, there will be less flow through $R_2$.
   \else
   \vspace{5em}
   \fi

3. If $R_1 \rightarrow 0$, what happens to $I_o$, $I_1$, and $I_2$?

   \ifsolutions
   **Answer**: $I_o \rightarrow \infty$, $I_1 \rightarrow \infty$, and $I_2\rightarrow 0$. In this case, we say that resistor $R_2$ is "shorted" because little current flows through it relative to $R_1$.
   \else
   \newpage
   \fi

%4. Suppose the two resistors were replaced with a resistor with a resistance of $1/\left(\frac{1}{R_1}+\frac{1}{R_2}\right)$ as shown below. What is $I_o$?

# Multiple Loops II

Assume the direction of currents $I_1$, $I_2$, and $I_3$ in the following circuit are as shown.

<img src="figures/Multiple_Loops_I.svg">

1. Write the equation for KVL for loop $A$.

   \ifsolutions
   **Answer**: $+\mathcal{E}-I_1R-I_3R=0$
   \else
   \vspace{3em}
   \fi

2. Write the equation for KVL for loop $B$.

   \ifsolutions
   **Answer**: $I_3R-I_2R=0$. A common error is to attempt to include $\mathcal{E}$ in this equation. When using KVL, the only elements that appear in the equation are elements that are stepped across when going around the chosen loop.
   \else
   \vspace{3em}
   \fi

3. Write the equation for KCL for junction X.

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
   \vspace{8em}
   \fi

5. Check your answers by plugging your values for $I_1$, $I_2$, and $I_3$ into the equations that you wrote for parts 1.-3.

   \ifsolutions
   **Comment**: This is an important step. Sign errors in KVL and KCL are common, as are algebraic errors, and this check will determine if you made an error.
   \else
   \newpage
   \fi

# Multiple Loops II

In the circuit for the previous problem, there are three possible loops. The third loop is loop $C$, which is indicated below.

<img src="figures/Multiple_Loops_II.svg">

1. Write the equation for KVL for loop $C$.

   \ifsolutions
   **Answer**: $\mathcal{E}-I_1R-I_2R=0$
   \else
   \vspace{3em}
   \fi

2. Use the equation for KVL for loop $B$ and the KCL equation for junction $X$ along with the KVL equation for loop $C$ to find $I_1$, $I_2$, and $I_3$ in terms of $\mathcal{E}$ and $R$. (You should get the same answers as the previous problem.)

\ifsolutions
\else
\newpage
\fi

# Redundant Equations

When solving circuit problems with multiple loops, you will generally find that you can use KVL and KCL to write more equations than there are unknown currents. If you attempt to solve a problem with $N$ unknowns by writing $N$ equations based on KVL and KCL but cannot solve for the unknowns, the reason is that two or more of the equations that you wrote were not independent. To demonstrate this, for the following circuit,

<img src="figures/Multiple_Loops_III.svg">

1. write the KCL equation for junction X,

   \ifsolutions
   **Answer**: $-I_1+I_2+I_3$
   \else
   \vspace{3em}
   \fi

2. write the KCL equation for junction Y,

   \ifsolutions
   **Answer**: $+I_1-I_2-I_3=0$
   \else
   \vspace{3em}
   \fi

3. write the KVL equation for loop $A$, and

   \ifsolutions
   **Answer**: $+\mathcal{E}-I_1R-I_3R=0$
   \else
   \vspace{3em}
   \fi
 
4. Is it possible to use the above three equations to solve for $I_1$, $I_2$, and $I_3$ in terms of $\mathcal{E}$ and $R$? If yes, do it. If no, explain why.

   \ifsolutions
   **Answer**: No. The equation for junction $X$ can be turned into the equation for junction $Y$ by multiplying all terms in it by $-1$. Thus, the equations are not independent. Given that three independent equations are needed to solve for three unknowns, a solution is impossible with the equations requested in parts 1.--3.
   \fi
