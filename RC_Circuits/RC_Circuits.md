```mdextension
Title: RC Circuits
```

# Notation and Equations

* We use the the letter "C" as a label for a capacitor and the units of charge. When used as a label, $C$ is usually written in itallics. Thus

  "$Q_C= 10 \text{ C}$" means "the capacitor labeled $C$ has a charge of $10$ Coulombs."

* Lower case letters are used for electrical quantities that vary in time. In circuits with only emfs and resistors, currents and voltages are constant, and we used $I$ and $V$. In the circuits considered in this activity, the currents and voltages vary in time, so we use $i(t)$ and $v(t)$.

* In this activity, we use the the relationship $i(t)=dq(t)/dt$ between the current $i(t)$ in the wires connected to a capacitor and the charge $q(t)$ on the capacitor.

# Discharging Capacitor

If one capacitor with capacitance $C$ is in a circuit with other resistors (and no emfs), the charge on the capacitor changes with time according to

$q(t)=Q_oe^{-t/\tau}$,

where $\tau\equiv RC$, $Q_o$ is the charge on the capacitor at $t=0$, and $R$ is the equivalent resistance. The quantity $\tau$ is called "RC time constant." The equation for $q(t)$ follows from using Kirchhoff's voltage law, which gives a differential equation, and then solving the differential equation.

## Problem

Find $\tau$ for the following two circuits. Use $R=10\text{ k}\Omega$ and $C=1\text{ }\mu\text{F}$.

<img src="figures/Discharging_a.svg"/>

\ifsolutions
**Answer**:
* Left: $R_{\text{eq}}=20\text{ k}\Omega$; $\tau = R_{\text{eq}}C = (20\cdot 10^3\text{ }\Omega) \cdot (10^{-6}\text{ F}) = 0.02\text{ s}$
* Right: $R_{\text{eq}}=5\text{ k}\Omega$; $\tau=.005\text{ s}$ 
\else
\vspace{1in}
\fi

\newpage
## Problem

For the following circuit, find the charge $q$ on the capacitor at $t=2\text{ s}$ if the switch is closed at $t=0$ and the capacitor has an initial charge of $Q_o$ for the following three cases.

1. $RC=1\text{ s}\qquad$ $q(2\text{ s})=\fbox{\qquad\phantom M}$

2. $RC=2\text{ s}\qquad$ $q(2\text{ s})=\fbox{\qquad\phantom M}$

3. $RC=4\text{ s}\qquad$ $q(2\text{ s})=\fbox{\qquad\phantom M}$

\ifsolutions
\else
\vspace{2cm}
\fi

Next, sketch a plot of $q(t)$ from $t=0$ to $t=6\text{ s}$ for each of these three cases. Used a solid, dashed, and dotted line for case 1., 2., and 3., respectively.

<img src="figures/Discharging_b.svg"/>

\ifsolutions
**Answer**:

$q(2)=Q_oe^{-2/RC}$, assuming $RC$ has units of seconds. So

1. $q(2)=Q_oe^{-2/1}=Q_o/e^2 \simeq 0.14 Q_o$

2. $q(2)=Q_oe^{-2/2}=Q_o/e \simeq 0.37 Q_o$

3. $q(2)=Q_oe^{-2/4}=Q_o/\sqrt{e} \simeq 0.61 Q_o$

All curves decay exponentially. To plot, start at $Q_o$, and draw an exponentially decaying curve that passes through one of the values above at $t=2$.
\fi

## Problem

<img src="figures/Discharging_c.svg"/>

In the circuit above, the values of $R$ and $C$ are such that $RC=1\text{ s}$.

1. If the capacitor has a charge of $10\text{ nC}$ and the switch is closed, how long will it take for the charge on the capacitor to fall to half of this value?

2. If the capacitor instead had a charge of $20\text{ nC}$ and the switch is closed, how long will it take for the charge on the capacitor to fall to half of this value?

\ifsolutions
**Answer**:

$q(t)=Q_oe^{-t/\tau}$ and we want $t$ when $q(t)=Q_o/2$, so need to solve 

$Q_o/2=Q_oe^{-t/\tau}\quad$ or $\quad 1/2=e^{-t/\tau}$

Taking the natural log of boths sides, and using $\ln(1/x)=-\ln x$, gives

$$-\ln(2) = \ln e^{-t/\tau} = -\frac{t}{\tau}$$

so $t=\tau\ln(2)\simeq 0.70\tau$. The answer does not depend on $Q_o$, so this is the answer for parts 1. and 2.
\else
\newpage
\fi

# Charging a Capacitor

If a single capacitor is in series with other resistors and a DC voltage source, the charge of the capacitor varies according to 

$$q(t)=Q_f(1-e^{-t/\tau})$$

where $\tau\equiv RC$, $R$ is the equivalent resistance, and $Q_f$ is the final charge on the capacitor, that is, the charge on the capacitor as $t\rightarrow\infty$ (it is technically more accurate to say $t\gg \tau$ instead of $t\rightarrow\infty$).

To find $Q_f$, replace the capacitor with an open circuit and use Kirchhoff's voltage law to find the voltage across the capacitor, $V_f$. Then use $Q_f=CV_f$.

## Example

Find $q(t)$ for the following circuit, assuming the switch is closed at $t=0$ and the capacitor is initially uncharged.

<img src="figures/Charging_a.svg"/>

**Answer**: When the switch is closed, charge builds up on the capacitor. This build--up continues until the charge on the capacitor is such that no current flows in the circuit. If no current flows through the capacitor, the circuit is equivalent to one in which the capacitor is replaced with an open circuit, as shown below. 

<img src="figures/Charging_b.svg"/>

Kirchhoff's voltage Law gives

$\mathcal{E}-i(t)R-v_C(t)=0$

For large $t$, $i(t)=0$, leaving $v_{C}(t)=\mathcal{E}$. This voltage is for large $t$, so we relabel it as $V_f$. Using $Q_f=CV_f$ gives $Q_f=C\mathcal{E}$, so

$$q(t)=C\mathcal{E}(1-e^{-t/RC})$$

Note that the general formula $q(t)=Q_f(1-e^{-t/\tau})$ that applies for all $t$ is derived by solving the differential equation $\mathcal{E}-i(t)R-v_C(t)=0$ using $i(t)=dq(t)/dt$ and $v_C(t)=Cq(t)$.

\ifsolutions
\else
\newpage
\fi

## Problem

For a circuit with any number of capacitors, DC voltage sources, and resistors, finding the equation for $q(t)$ for each capacitor requires solving a system of differential equations, which is not covered in this course. However, you can find the currents and charges on the capacitor after a long time by replacing all capacitors with open circuits and then using KVL.

<img src="figures/Charging_c.svg"/>

1. Find the charge on the capacitor a long time after the switch is closed. 
2. Find the current in the resistor a long time after the switch is closed.

\ifsolutions
**Answer**
1. $Q_f=\mathcal{E}C$
2. $i_{Rf}=\mathcal{E}/R$
\else
\vspace{2in}
\fi

\newpage
# Charge/Discharge Problem

## Part I

<img src="figures/Charge_Discharge_a.svg"/>

The switch in the above circuit has been in position $a$ for a long time. At $t = 0$, the switch is moved to position $b$. The values of the circuit elements are $\mathcal{E}= 12\text{ V}$, $C = 10\text{ mF}$, and $R = 20\text{ }\Omega$.

Let $t=0^-$ correspond to the time just before the switch is moved from $a$ to $b$. Let $t=0^+$ correspond to the time just after the switch is moved from $a$ to $b$.

1. What is the current through the resistor at $t=0^-$?

   \ifsolutions
   **Answer**: Zero.
   \else
   \vspace{2cm}
   \fi

2. What is the current through the resistor at $t=0^+$?

   \ifsolutions
   **Answer**: Immediately after the switch is moved to $b$, the capacitor starts to discharge though the resistor. Kirchhoff's Voltage law states that the voltage across the resistor equals the voltage across the capacitor, $v_C$. By Ohm's law current through the resistor is $i(0^+) = v_C(0^+)/R = 12\text{ V}/20\text{ }\Omega = 0.6\text{ A}$.
   \else
   \vspace{2cm}
   \fi

3. What is the charge on the capacitor at $t=0^-$?

   \ifsolutions
   **Answer**: $q(0^-) = Cv_C(0^-) = (10 \text{ mF})(12\text{ V}) = 120\text{ mC}$.
   \else
   \vspace{2cm}
   \fi

4. What is the charge on the capacitor at $t=0^+$?

   \ifsolutions
   **Answer**: $120\text{ mC}$
   \else
   \vspace{2cm}
   \fi

5. What is the charge on the capacitor at $t = 200\text{ ms}$?

   \ifsolutions
   {\bf Answer: } The time constant is $RC= (10\text{ mF}) (20\text{ }\Omega) = 200\text{ ms}$. At $t = 200\text{ ms}$, the capacitor is in the process of discharging. The charge on the capacitor varies according to $q(t)=Q_oe^{-t/RC}$, so

   $q(200\text{ ms}) = Q_0e^{-200\text{ ms}/RC} = 120\text{ mC} \cdot e^{-200\text{ ms}/200\text{ ms}} \simeq120\text{ mC}\cdot 0.37 \simeq 44 \text{ mC}$.
   \else
   \vspace{2cm}
   \fi

\newpage
## Part II

<img src="figures/Charge_Discharge_b.svg"/>

The switch in the above circuit has been in position $b$ for a long time. At $t = 0$, the switch is moved to position $a$. The values of the circuit elements are $\mathcal{E}= 12\text{ V}$, $C = 10\text{ mF}$, and $R = 20\text{ }\Omega$.

Let $t=0^-$ correspond to the time just before the switch is moved from $b$ to $a$. Let $t=0^+$ correspond to the time just after the switch is moved from $b$ to $a$.

1. What is the current through the resistor at $t=0^-$?

   \ifsolutions
   {\bf Answer: } Since the switch is on position $b$ for a long time, the charge on and voltage across the capacitor is zero. If the voltage across the capacitor is zero, then by Kirchhoff's voltage law, the voltage across the resistor must be zero. So the current through the resistor is zero.
   \else
   \vspace{2cm}
   \fi

2. What is the voltage across the capacitor at $t=0^-$?

   \ifsolutions
   {\bf Answer: } Zero.
   \else
   \vspace{2cm}
   \fi

3. What is the charge on the capacitor at $t=0^-$?

   \ifsolutions
   {\bf Answer: } Zero.
   \else
   \vspace{2cm}
   \fi

4. What is the charge on the capacitor at  $t=0^+$?

   \ifsolutions
   {\bf Answer: } Zero.
   \else
   \vspace{2cm}
   \fi

5. What is the current through the resistor at $t=0^+$?

   \ifsolutions
   {\bf Answer:} Kirchhoff's voltage law at this time is

   $\mathcal{E}-i(0^+)R-v_C(0^+)=0$

   At $t=0^+$ the voltage across the capacitor is zNeero because it is uncharged, so $i(0^+)R=\mathcal{E}$. Thus, $i(0^+) = \mathcal{E}/R = 12\text{ V}/20\text{ }\Omega = 0.6\text{ A}$.
   \else
   \vspace{2cm}
   \fi

6. What is the charge on the capacitor at time $t = 200\text{ ms}$?

   \ifsolutions
   {\bf Answer: } The time constant is $RC=200\text{ ms}$. At $t=200\text{ ms}$, the charge accumulated on the capacitor is:

   $$q(200\text{ s}) = C\mathcal{E}(1-e^{-(200\text{ s})/RC}) = (10\text{ mF} \cdot 12\text{ V})(1-e^{-200/200})\simeq (120\text{ mV})(0.63)\simeq 75.9\text{ mV}$$
   \else
   \fi
