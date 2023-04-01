# Introduction

This activity involves circuits with DC voltage supplies (e.g., batteries), resistors and capacitors.

There are generally three types of problems for such circuits:

I. A single capacitor is charged and placed in a circuit with other resistors (and no batteries).

II. Finding currents and voltages just before and just after a switch is closed in a circuit with DC voltage supplies (e.g., batteries), resistors and capacitors.

III. Finding the time dependence of currents and voltages after a switch is closed. 

The third type of problem is the most general and problems of type I and type II can be solved using the method demonstrated for type III problems.

# Type I

From the definition of capacitance, $C=Q/V$, the voltage across a capacitor is $V=Q/C$. Kirchhoffs voltage law for the following circuit is 

$$IR+V_c=IR+Q/C=0$$

Suppose that we want to know $I$ and $R$ and $C$ are given. This equation would appear to have two unknows, $I$ and $Q$ and so to find $I$, we need another equation. We know that the current $I$ is related to charge according to $I=dQ/dt$. This leaves

$\ds R\frac{dQ}{dt}+\frac{Q}{C}=0\quad$ or
$\quad\ds\frac{dQ}{dt}+\frac{Q}{RC}=0$

So solve for $I$, we first need to know $dQ/dt$. The above is an ordinary differential equation that has solution of

$Q(t)=Q_oe^{-t/\tau}$, where $\tau\equiv RC$ and $Q_o$ is the charge on the capacitor at $t=0$.

## Problem

1. Show that $Q=Q_oe^{-t/\tau}$ with $\tau\equiv RC$ satisfies 

   $\ds\frac{dQ}{dt}+\frac{Q}{RC}=0$

2. If $Q_o$ is doubled, does $Q=Q_oe^{-t/\tau}$ still satisfy the above equation?

This equation 

$Q(t)=Q_oe^{-t/\tau}$, where $\tau\equiv RC$ and $Q_o$ is the charge on the capacitor at $t=0$ applies to any circuit with only a single capacitor and one or more resistors. If there is more than one resistor, $R$ is the equivalent resistance.

## Example

Find $Q(t)$ after the switch is closed for the following circuit.

## Problem

Find $Q(t)$ after the switch is closed for the following circuit.

## Problem

If $Q(t)=Q_oe^{-t/\tau}$ and

1. $Q_o=1\text{ nF}$ and $RC=1\text{ s}$

2. $Q_o=1\text{ nF}$ and $RC=2\text{ s}$

3. $Q_o=1\text{ nF}$ and $RC=4\text{ s}$

find $Q$ at $t=1\text{ s}$. Enter your answers below

1. 
2. 
3. 

Next sketch a plot of $Q(t)$ from $t=0$ to $t=8\text{ s}$. Used a solid, dashed, and dotted line for case 1., 2., and 3., respectively.

## Problem

1. If the capacitor has a charge of $10\text{ nC}$ and the switch is closed, how long will it take for the charge on the capacitor to fall to half of its value?

2. If the capacitor instead had a charge of $20\text{ nC}$ and the switch is closed, how long will it take for the charge on the capacitor to fall to half of its value?

# Type II

If a circuit is configured such that no current can flow through an uncharged capacitor and then a switch is closed such that current can flow, the current in all parts of the circuit can be found at the instant the switch is closed by replacing the capacitor with a zero resistance wire.

After a long time, the currents and voltages in the circuity can be found by replacing the capacitor with an open circuit.

## Example

## Problem

\item The circuit above has been in position {\bf a} for a long time. At time t = 0 the switch is thrown to position {\bf b}. The values of circuit elements are: V$_b$ = 12 V, C = 10 mF, R = 20$\Omega$
\\
\par a. What is the current through the resistor just {\bf before} the switch is thrown?

    \ifsolutions
    {\bf Answer: } Just before the switch is thrown, the current across the capacitor and around this circuit is 0 (the capacitor is fully charged and no more charges can be further accumulated on the capacitor. Since the current through the resistor is zero, the voltage across the capacitor equals the voltage of the power source, $V_C = V_b = 12 V$.
    \else
    \\
\vspace{0.5cm}
\fi
   
\par b. What is the current through the resistor just {\bf after} the switch is thrown?

    \ifsolutions
    {\bf Answer: }Immediately after the switch is thrown, the capacitor starts to discharge though the resistor. By Kirchhoff's loop rule, the voltage across the resistor equals V$_C$. The current through the resistor is I = V$_C$/ R = 12/20 = 0.6 A
    \else
   \\
\vspace{0.5cm}
\fi
   
\par c. What is the charge on the capacitor just {\bf before} the switch is thrown?

    \ifsolutions
    {\bf Answer: }  Just before the switch is thrown the charge on the capacitor is: Q = CV = (10mF)(12 V) = 120 mC  
    \else
   \\
\vspace{0.5cm}
\fi
   
\par d. What is the charge on the capacitor just {\bf after} the switch is thrown?

    \ifsolutions
    {\bf Answer: }  Just after the switch is thrown, the change of the stored charge is zero at t=0. The charge on the capacitor just after the switch is thrown remains 120 mC.
    \else
   \\
\vspace{0.5cm}
\fi
   
\par e. What is the charge on the capacitor at time t = 0.3 msec after the switch is thrown?

    \ifsolutions
    {\bf Answer: } The time constant for the RC circuit is RC= (10mF) (20 ohm) = 200 msec. At t = 0.3 msec after the switch is thrown to b, the capacitor is in the process of discharging. The charge on the capacitor:
    
    $$Q = Q_0e^{-t/RC} = 120 mC \times e^{-0.3/200} = 119.8 mC$$
    
    \else
   \\
\vspace{0.5cm}
\fi
   
\item Considering the same circuit, only with the switch thrown from {\bf b} to {\bf a} at time t = 0 after having been in position {\bf b} for a long time. Data: V$_b = 12$ V, C = 10 mF, R = 20$\Omega$
\\
\vspace{0.1cm}
   
\par a. What is the current through the resistor just {\bf before} the switch is thrown?

    \ifsolutions
    {\bf Answer: }  Since the switch is on position b for a long time, the charge across the capacitor is 0 (fully discharged). There is no current in the circuit, that is, the current through the resistor is 0.  
    \else
   \\
\vspace{0.5cm}
\fi
   
\par b. What is the current through the resistor just {\bf after} the switch is thrown?

    \ifsolutions
    {\bf Answer: }  Just after the switch is thrown to position a, the voltage across the capacitor is 0, and the voltage across the resistor is V$_b$. From Ohm’s law, the current through the resistor is $I = V_b/R = 12V/20 \Omega = 0.6A$.  
    \else
   \\
\vspace{0.5cm}
\fi
   
\par c. What is the charge on the capacitor just {\bf before} the switch is thrown?

    \ifsolutions
    {\bf Answer: }  Before the switch is thrown, the charge on the capacitor is 0.
    \else
   \\
\vspace{0.5cm}
\fi
   
\par d. What is the charge on the capacitor just {\bf after} the switch is thrown?

    \ifsolutions
    {\bf Answer: }  The charge on the capacitor just after the switch is thrown remains zero.
    \else
   \\
\vspace{0.5cm}
\fi
   
\par e. What is the charge on the capacitor at time t = 0.3 msec after the switch is thrown?

    \ifsolutions
    {\bf Answer: } After the switch is thrown, the capacitor is in a charging process. The time constant is RC=200 msec. At time=0.3, the charge accumulated on the capacitor is:
       
       $$Q = CV_b[1-e^{t/RC}] = 10 mF \times 12V[1-e^{-0.3/200}] = 0.18 mC$$
    \else
   \fi
   
    \end{enumerate}

\end{tcolorbox}
