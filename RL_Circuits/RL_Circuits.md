```mdextension
Title: RL Circuits
```

# Introduction

<img src="figures/LR_Series.svg">

The above figure shows a RL series circuit consisting of an inductor of inductance $L$ connected in series with a resistor of resistance $R$. The switch, $S$, is closed at a time $t = 0$ and remains closed.

Using Kirchhoff’s voltage law around the loop, we have

$$
V_s - I(t) \cdot R - L \frac{dI(t)}{dt} = 0
$$

This differential equation can be solved for $I(t)$, the current at any time. If the current at $t=0$ is zero, the solution is

$$
I(t)=\frac{V_s}{R}\left(1-e^{-t/(L/R)}\right)
$$

After a long time$^*$ (specifically, $t\gg\tau$), the current approaches a constant value of $I = V_s/R$ because the exponential term approaches zero. How quickly the exponential term approaches zero depends on a quantity called the RL time constant defined by

$$\tau \equiv L/R$$

which has units of seconds when $L$ is in Henrys ($\text{H}$) and $R$ is in Ohms ($\Omega$). Using $\tau$, we have

$$
I(t) = \frac{V_s}{R}\left(1-e^{-t/\tau}\right)
$$

When $t/\tau \simeq 0$, $e^{-t/\tau} \simeq e^0 = 1$, so $I(t) \simeq (V_s/R)(1-1)=0$. As a result, we state that initially the inductor behaves like an open circuit because the current through it is nearly zero.

When $t/\tau \gg 1$, the exponential term $e^{-t/\tau}$ becomes much smaller than one, so $I(t) \simeq (V_s/R)(1-0)=V_s/R$. If we replace the inductor with a wire, this is the same current that we would find. As a result, we state that after a long time, an inductor behaves like a resistanceless wire.

$^*$ Informally, we often use phrases such as "after a long time". This phrase is ambiguous because a reference length of time is not given. To be specific, one should instead state $t\gg t_{\text{ref}}$, where $t_{\text{ref}}$ is a reference length of time.

\newpage

# Problem I

In this problem, you will consider the circuit and equation

$$I(t) = \frac{V_s}{R}\left(1-e^{-t/\tau}\right)$$

that was described in the introduction.

1. If $V_s = 10\text{ V}$ and $R=1\text{ }\Omega$, plot dots for the values of $I$ at $t=0, 2, 4, 6, 12\text{ s}$ using $L/R = \tau = 2\text{ s}$ 

   \ifsolutions
   <img src="figures/I_vs_t_Solution.svg" width="200px">
   \else
   <img src="figures/I_vs_t.svg">
   \fi

2. Based on the equation, at $t=0$ does the inductor behave like an open circuit or a resistanceless wire?

   \ifsolutions
   {\bf Answer}: At $t=0$ the current will be zero, which is the same current that would be found if the inductor was removed and the wires that were connected to the inductor were left disconnected (so an open circuit).
   \else
   \vspace{1em}
   \fi

3. Based on the equation, at $t\gg \tau$ does an inductor behave like an open circuit or a resistanceless wire?

   \ifsolutions
   {\bf Answer}: When $t \gg \tau$ the current is approximately $V_s/R$, which is the same current that would be found if the inductor was replaced with a resistanceless wire.
   \else
   \vspace{2em}
   \fi
    
3. If $L$ doubles but $R$ remains constant
    
   a. does the time constant $\tau$ increase, decrease, or remain the same?;

   \ifsolutions
   {\bf Answer}: $\tau=L/R$, so $\tau$ doubles.
   \else
   \vspace{2em}
   \fi

   b. how will the position of the points that you drew for part 1. change? (Will they move up, down, or remain the same?) 

   \ifsolutions
   {\bf Answer}: All points move down except the point at $t=0$.
   \else
   \vspace{2em}
   \fi

   c. Does your answer to b. make sense physically? That is, an inductor tends to impede changes in current and so is your answer to b. consistent with this? 

   \ifsolutions
   {\bf Answer}: If $L$ increases, the inductor provides more opposition to change in the currrent through it. Thus we expect the current to take longer to reach its final state.
   \else
   \vspace{2em}
   \fi

4. The voltage across the inductor is $LdI/dt$. Compute $dI/dt$ and sketch its curve on the graph above. Is this equation consistent with the statement that for large $t/\tau$, the voltage across the inductor is zero?

   \ifsolutions
    {\bf Answer:} $LdI/dt = V_se^{-t/\tau}$. Yes. The voltage across the inductor is $V_se^{-t/\tau}$ and for large $t/\tau$, $e^{-t/\tau}$ is small.
   \else
   \newpage
   \fi

# Problem II

If the circuit in the introduction has $L=40\text{ mH}$, $R=2\text{ }\Omega$, and $V_s=20\text{ V}$,

1. What is the current after a very long time after the switch is closed?

   \ifsolutions
   {\bf Answer}: $I = V_s/R=(20\text{ V})/(2\text{ }\Omega) = 10\text{ A}$
   \else
   \vspace{5em}
   \fi

2. What is the time constant of this RL series circuit?

   \ifsolutions
   {\bf Answer}: $\tau = L/R = (40\text{ mH})/(2\text{ }\Omega) = 20 \text{ ms}$
   \else
   \vspace{5em}
   \fi

3. How long does it take for the current to reach $63$\% of its maximum value?

   \ifsolutions
   {\bf Answer}: The current in the circuit is expressed as:

   $$
   I(t)=  \frac{V_s}{R}\left(1-e^{-t/\tau}\right)
   $$

   The maximum current value is $I_{\text{max}}=V_s/R$. Therefore,

   $$
   \frac{I(t)}{I_{\text{max}}} = 1-e^{-t/\tau}
   $$

   Setting $I(t)/I_{\text{max}} =0.63\quad$ gives $\quad0.63 = 1-e^{-t/\tau}\quad\Rightarrow\quad e^{-t/\tau} = 1-0.63 = 0.37$

   $e^{-t/\tau} = 0.37\quad\Rightarrow\quad -t/\tau = \ln(0.37)=-0.9943\quad\Rightarrow\quad t = 19.89\text{ ms}$

   Thus, it takes roughly $20\text{ ms}$ ($\simeq \tau$) to reach $63$\% of the maximum current value. (So $0.63$ is a special number for an RL circuit -- at $t=\tau$, the current is $\simeq 63$\% of its maximum value.)
   \else
   \vspace{15em}
   \fi

4. What is the voltage across the inductor at $t = 10\text{ ms}$?

   \ifsolutions
   {\bf Answer}: From part 5. of the previous problem, $v_L(t)=LdI/dt = V_se^{-t/\tau}$, so

   $v_L(10\text{ ms}) = (20\text{ V})e^{-10/20}\simeq 12.1\text{ V}$
   \else
   \vspace{5em}
   \fi

5. What is the current at $t=\tau$ after the switch is closed?

   \ifsolutions
   {\bf Answer}: At time $t = \tau$,

   $$
   I(\tau) = \frac{V_s}{R} (1-e^{-\tau/\tau}) = (10\text{ A})(1-0.368) = 6.32\text{ A}
   $$

   This question is related to question 3. In the answer to question 3., it was found that it takes approximately one time constant for the current to reach $63$\% of the maximum value.
   \else
   \fi

\newpage

# Problem III

<img src="figures/LR_Two_Switches.svg">

In the circuit above, an inductor with $L=10\text{ mH}$ and a resistor with $R=1\text{ }\Omega$ is connected as shown. The battery has an emf of $10\text{ V}$. At $t=0$, the switch $S_1$ is closed.


1. What is the current through the resistor at $t=0$?

   \ifsolutions
   {\bf Answer}: Zero. There is no closed path for current to flow.
   \else
   \vspace{1em}
   \fi

2. What is the current through the inductor at $t=0$?

   \ifsolutions
   {\bf Answer}: Zero. There is no closed path for current to flow.
   \else
   \vspace{1em}
   \fi

3. After a long time, what is the current through the resistor and inductor?

   \ifsolutions
   {\bf Answer}: The current in the circuit as a function of time is

   $$
   I(t) =  \frac{V_s}{R}\left(1-e^{-t/(L/R)}\right)
   $$

   For large $t$, the exponential term is near zero, leaving $V_s/R=10\text{ V}/1 \text{ }\Omega$ = $10\text{ A}$.
   \else
   \vspace{3em}
   \fi

4. $S_1$ is opened and $S_2$ is closed simultaneously at $t=t_o$. Write Kirchhoff's voltage law around the new closed loop.

   \ifsolutions
   {\bf Answer}: $\ds -I(t) R - L\frac{dI(t)}{dt} = 0$
   \else
   \vspace{3em}
   \fi

5. Show that the equation $I(t)=I_oe^{-(t-t_o)/\tau}$ satisfies the equation in your answer to the previous question.

   \ifsolutions
   {\bf Answer}: Starting with

   $$-I(t) \cdot R - L \frac{dI(t)}{dt} = 0$$

   and using
   
   $$I=I_oe^{-(t-t_o)/\tau}$$
   
   and
   
   $$\frac{d}{dt}\left(e^{-(t-t_o)/\tau}\right) = -\frac{1}{\tau} e^{-(t-t_o)/\tau}$$

   we have

   $$-I_oe^{-(t-t_o)/\tau} \cdot (1\text{ }\Omega) + (10\text{ mH}/\tau)e^{-(t-t_o)/\tau} = 0$$

   Using $\tau = L/R$ one arrives at

   $-I_oe^{-(t-t_o)/\tau} + I_oe^{-(t-t_o)/\tau} = 0$.
   \else
   \vspace{5em}
   \fi

6. If switch $S_1$ was opened and switch $S_2$ was closed at $t_o=5\text{ ms}$, plot $I(t)$ from $t=0$ to $t=10\text{ ms}$.

   \ifsolutions
   In the range $t=[0, 5]\text{ ms}$, $I(t) = (10\text{ A})\left(1-e^{-t/\tau}\right)$. At $t=5\text{ ms}$,

   $I(5\text{ ms}) = (10\text{ A})\left(1-e^{-5\text{ ms}/10\text{ ms}}\right) \approx 4\text{ A}$

   For $t\ge 5\text{ ms}$, the solution $I(t) = I_o e^{-(t-t_o)/\tau}$
   
   Because the current is continuous at $t=5\text{ ms}$, $I_o = 4\text{ A}$.
   
   A plot of

   $I(t) = (10\text{ A})\left(1-e^{-t/\tau}\right)$ for $t=[0, 5]\text{ ms}$
   
   and
   
   $I(t) = (10\text{ A})e^{-(t-5\text{ ms})/\tau}$ $t\ge 5\text{ ms}$ is shown below.
   
   
   <img src="figures/I_vs_t_SolutionIII.svg" width="200px">
   \else
   <img src="figures/I_vs_t.svg">
   \fi
