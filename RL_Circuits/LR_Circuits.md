```mdextension
Title: LR Circuits
```

# Introduction

<img src="figures/LR_Series.svg">

The above figure shows a LR series circuit consisting of an inductor $L$ connected in series with a resistor $R$. The switch, $S$, is closed at a time $t = 0$ and then remains closed. 

Using Kirchhoff’s voltage law around the loop, we have

$$
V_s - I(t)R - L \frac{dI(t)}{dt} = 0
$$

The term $L dI/dt$ is called the induced emf. The above differential equation can be solved for $I(t)$, the current at any time given its initial value, $I(0)$, which is zero. The result is

$$
I(t)=\frac{V_s}{R}\left(1-e^{-t/(L/R)}\right)
$$

After a long time, ($t\gg L/R$) the current approaches a constant value of $I = V_s/R$ because the exponential term approaches zero. How quickly the exponential term approaches zero depends on a quantity called the LR time constant, $\tau$, defined by

$$\tau = L/R$$

which has units of seconds when $L$ is in Henrys ($\text{H}$) and $R$ is in Ohms ($\Omega$). With this, we can write

$$
I(t) = \frac{V_s}{R}\left(1-e^{-t/\tau}\right)
$$

In this equation, at $t=0$, the current is

$$
I(0) = (V_s/R)\left(1-e^{-0/\tau}\right)=(V_s/R)\left(1-1\right)=0
$$

As a result, we state that initially the inductor behaves like an open circuit because current does not flow though it.

For large $t/\tau$, the exponential term becomes much smaller than one and so the current becomes a constant value of $V_s/R$. If we replace the inductor with a wire, this is the same current that we would find. As a result, we state that after a long time, the inductor behaves like a resistanceless wire.

\ifsolutions
\else
\newpage
\fi

# Problem I

In this problem, you will consider the equation

$$I(t) = \frac{V_s}{R}\left(1-e^{-t/\tau}\right)$$

that was described in the introduction.

1. If $V_s/R=10\text{ A}$, plot dots for the values of $I$ at $t=0, 2, 4, 6, 12\text{ s}$ with $L/R = \tau = 2\text{ s}$ 

  <img src="figures/I_vs_t.svg">

2. Based on the given equation for $I(t)$, at $t=0$, does an inductor behave like an open circuit or a wire?
    
  \ifsolutions
  **Answer**: At $t=0$ the current will be $0$ with the inductor acting like a break in the circuit with no current flowing.
  \else
  \vspace{2em}
  \fi

3. Based on the equation, for $t\gg \tau$, does an inductor behave like an open circuit or a wire?

  \ifsolutions
  **Answer**: For $t \gg \tau$, the current will be approximately $V_s/R$, which is the same current found if the inductor is replaced with a wire with no resistance.
  \else
  \vspace{2em}
  \fi

4. If $L$ doubles but $R$ remains constant,

   * does the time constant $\tau$ increase, decrease, or remain the same?;

     \ifsolutions
     **Answer**: Increase by a factor of $2$.
     \else
     \vspace{2em}
     \fi

   * how will the points that you drew for part 1. change? (Will they move up, down, or remain the same?); and

     \ifsolutions
     **Answer**: All of the points except for $t=0$ will move downward.
     \else
     \vspace{2em}
     \fi

   * does your answer to b. make sense physically? That is, an inductor tends to impede changes in current and so is your answer to b. consistent with this? 

     \ifsolutions
     **Answer**: If $L$ increases, the inductor provides more resistance to change from its initial state, which is $I=0$. Thus, we expect the current to take longer to reach its final state.
     \else
     \vspace{2em}
     \fi

5. The voltage across the inductor is $LdI/dt$. Compute $dI/dt$ and sketch its curve on the plot of part 1. Is this equation consistent with the statement that for large $t/\tau$, the voltage across the inductor is zero?

  \ifsolutions
  **Answer**: $LdI/dt = -V_se^{-t/\tau}$. Yes. The voltage across the inductor is $-V_se^{-t/\tau}$ and for large $t/\tau$, $e^{-t/\tau}$ is near zero.
  \else
  \newpage
  \fi

# Problem II

An inductor with an inductance of $40\text{ mH}$, a resistor with a resistance of $2\text{ }\Omega$, and a $20\text{ V}$ DC voltage source are connected in series. Include units in all of your answers.

1. What will be the final steady-state value of the current (the current after a very long time)?

   \ifsolutions
   **Answer**: At the steady state, the current passing through the inductor is constant, and the induced emf becomes 0. Consequently, the voltage drop on the resistor is the same as the total voltage of the DC supply.

   $$I = V_s/R=(20\text{ V})/(2\text{ }\Omega) = 10\text{ A}$$
  \else
  \vspace{5em}
  \fi

2. What is the time constant of the RL series circuit?

   \ifsolutions
   **Answer**: The time constant is given by $\tau = L/R = (40\text{ mH})/(2\text{ }\Omega) = 20 \text{ ms}$
   \else
   \vspace{5em}
   \fi

3. How long does it take for the current to reach 63\% of its maximum value?

   \ifsolutions
   **Answer**: The current in the circuit is expressed as:

   $$I(t) = \frac{V_s}{R}\left(1-e^{-t/(L/R)}\right)$$

   The maximum current value is $I_0=V_s/R$. Therefore,

   $$\frac{I(t)}{I_0} = 1-e^{-t/(L/R)} = 1-e^{-t/\tau}$$

   When $I(t)/I_0 =0.63$ and $\tau = L/R = 40\text{ ms}$:

   $$0.63 = 1-e^{-t/\tau}\Rightarrow\quad e^{-t/\tau} = 1-0.63 = 0.37$$

   $$-t/\tau = \ln(0.37) = -0.9943\quad\Rightarrow\quad t = 19.89\text{ ms}$$

   It takes approximately $20\text{ ms}$ ($\simeq \tau$) to reach $63$\% of the maximum current value. (So $0.63$ is a special number for an LR circuit -- at $t=\tau$, the current is $0.63$ of its maximum value.)
   \else
   \vspace{5em}
   \fi

4. What will be the value of the induced emf after $10\text{ ms}$?

   \ifsolutions

   **Answer**: After 10 ms, the current is calculated as:

   $$
   I(10\text{ ms}) = \frac{20 \text{ V}}{2\text{ }\Omega} \left(1-e^{-(10\text{ ms})/(20\text{ ms})}\right) = 3.9\text{ A} 
   $$

   The induced emf is:

   $$
   \text{emf} = V_s - IR= 20\text{ V} - 3.9\text{ A} \cdot 2~\Omega=12.2\text{ V} 
   $$
   \else
   \vspace{5em}
   \fi

4. What will be the value of the circuit current one-time constant (that is, at $t=\tau$) after the switch is closed?

   \ifsolutions

   **Answer**: At time $t = \tau$,

   $$I(\tau) = 10(1-0.368) = 6.32\text{ A}$$

   This question is related to question 3. In the answer to question 3., it was found that it takes approximately one time constant to reach $63$\% of the maximum value. So, in this problem, we expect the answer to be approximately $63$\% of the final value.
   \else
   \newpage
   \fi

# Problem III

<img src="figures/LR_Two_Switches.svg">

In the circuit above, an inductor with $L=10\text{ mH}$ and a resistor with $R=1\text{ }\Omega$ is connected as shown. The battery has an emf of $10\text{ V}$. At $t=0$, the switch $S_1$ is closed.


1. What is the current through the resistor at $t=0$?

   \ifsolutions
   **Answer**: Zero. There is no closed path for current to flow.
   \else
   \vspace{3em}
   \fi

2. What is the current through the inductor at $t=0$?

   \ifsolutions
   **Answer**: Zero. There is no closed path for current to flow.
   \else
   \vspace{3em}
   \fi

3. After a long time, what will the current be through the resistor and inductor?

   \ifsolutions
   **Answer**: The current in the circuit as a function of time is

   $$
   I(t)=  \frac{V_s}{R}\left(1-e^{-t/(L/R)}\right)
   $$

   For large $t$, the exponential term is near zero, leaving $V_s/R=10\text{ V}/1 \text{ }\Omega$ = $10\text{ A}$.
   \else
   \vspace{3em}
   \fi

4. Switch $S_1$ is opened and $S_2$ is closed simultaneously at $t=0.005\text{ s}$. Write Kirchhoff's voltage law around the new closed loop.

   \ifsolutions
   **Answer**:

   $$-I(t)R - L \frac{dI(t)}{dt} = 0$$
   \else
   \vspace{3em}
   \fi

5. Show that the equation $I(t)=(10\text{ A})e^{-t/\tau}$ satisfies the equation in your answer to the previous question.

   \ifsolutions

   If $I(t)=10e^{-t/\tau}$,
   
   $$\frac{dI(t)}{dt}= \frac{d 10e^{t/\tau}}{dt} = \frac{1}{\tau} e^{-t/\tau}$$

   Substitution into
   
   $$-I(t)R - L \frac{dI(t)}{dt} = 0$$

   gives

   $$-(10\text{ A})e^{-t/\tau} \cdot (1\text{ }\Omega) - (10\text{ mH}/\tau)e^{-t/\tau} = 0$$

   Using $\tau = L/R$ one arrives at

   $$-(10\text{ V})e^{-t/\tau} - (10\text{ V})e^{-t/\tau} = 0$$

   As a result, $I(t)=10e^{-t/\tau}$ satisfies Kirchhoff's voltage law.
   \else
   \vspace{3em}
   \fi

6. Plot $I(t)$ from $t=0$ to $t=0.01\text{ s}$. (Switch $S_1$ was opened and switch $S_2$ was closed at $t=0.005\text{ s}$).

   <img src="figures/I_vs_t.svg">
