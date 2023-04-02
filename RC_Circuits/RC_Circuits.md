```mdextension
Title: Capacitance
```

# Notation and Equations

We use the the letter "C" as a label for a capacitor and in the units of capacitance. When used as a label, $C$ is usually written in itallics. Thus

"$C= 10 \text{ C}$" means "the capacitor labeled $C$ has a capacitance of $10$ Coulombs.

Lower case letters are used for electrical quantities that vary in time. In circuits where there were only emfs and resistors, currents and voltages are constant and we use $I$ and $V$. In the circuits considered in this activity, the currents and voltages vary in time, so we use $i(t)$ and $v(t)$.

In this activity, we also use the the relationship between the current $i$ in the wires connected to a capacitor and the charge $q$ on the capacitor is $i=dq/dt$.

# Discharging Capacitor

If a single charged capacitor with capacitance $C$ is in a circuit with other resistors (and no emfs), the charge on the capacitor changes with time according to

$q(t)=Q_oe^{-t/\tau}$,

where $\tau\equiv RC$, $Q_o$ is the charge on the capacitor at $t=0$, and $R$ is the equivalent resistance. The quantity $\tau$ is often referred to as the "RC time constant". This equation follows from using Kirchhoff's voltage law, which gives a differential equation, and then solving the differential equation.

## Problem

Find $\tau$ for the following two circuits. Use $R=10\text{ k}\Omega$ and $C=1\text{ }\mu\text{F}$.

<img src="figures/Discharging_I.svg"/>

**Answer**: Left: $R_{\text{eq}}=20\text{ k}\Omega$; $\tau = R_{\text{eq}}C = 20\cdot 10^3 \times 10^{-6}\text{ s}=.02\text{ s}$. Right: $R_{\text{eq}}=5\text{ k}\Omega$; $\tau=.005\text{ s}$ 

\ifsolutions
\else
\fi

## Problem

For the following circuit, find the charge $q$ on the capacitor at $t=2\text{ s}$ if the switch is closed at $t=0$ and the capacitor has an inital charge of $Q_o$ for the following three cases.

1. $RC=1\text{ s}\qquad$ $q(t=2\text{ s})=\fbox{\qquad\phantom M}$

2. $RC=2\text{ s}\qquad$ $q(t=2\text{ s})=\fbox{\qquad\phantom M}$

3. $RC=4\text{ s}\qquad$ $q(t=2\text{ s})=\fbox{\qquad\phantom M}$

Next sketch a plot of $q(t)$ from $t=0$ to $t=6\text{ s}$ for each of these three cases. Used a solid, dashed, and dotted line for case 1., 2., and 3., respectively.

<img src="figures/Discharging_II.svg"/>

**Answer**:

$q(2)=Q_oe^{-2/RC}$, assuming $RC$ has units of seconds. So

1. $q(2)=Q_oe^{-2/1}=Q_o/e^2 \simeq 0.14 Q_o$

2. $q(2)=Q_oe^{-2/2}=Q_o/e \simeq 0.37 Q_o$

3. $q(2)=Q_oe^{-2/4}=Q_o/\sqrt{e} \simeq 0.61 Q_o$

All curves decay exponentially, start at $Q_o$, and pass through one of the values above $t=2$.

\ifsolutions
\else
\fi

## Problem

<img src="figures/Discharging_III.svg"/>

In the circuit above, the values of $R$ and $C$ are such that $RC=\tau=1\text{ s}$.

1. If the capacitor has a charge of $10\text{ nC}$ and the switch is closed, how long will it take for the charge on the capacitor to fall to half of its value?

2. If the capacitor instead had a charge of $20\text{ nC}$ and $RC=1\text{ s}$ and the switch is closed, how long will it take for the charge on the capacitor to fall to half of its value?

**Answer**:

$q(t)=Q_oe^{-t/\tau}$ and we want $t$ when $q(t)=Q_o/2$, so need to solve 

$$Q_o/2=Q_oe^{-t/\tau}$$

or

$$1/2=e^{-t/\tau}$$

Taking the natural log of boths sides, and using $\ln(1/x)=-\ln x$, gives

$$-\ln(2) = \ln e^{-t/\tau} = -\frac{t}{\tau}$$

so $t=\tau\ln(2)\simeq 0.70\tau$. The answer does not depend on $Q_o$, so this is the answer for parts 1. and 2.

%\ifsolutions
%\else
%\fi

# Charging a Capacitor

If a single capacitor is in a circuit with other resistors and an DC voltage source, the charge of the capacitor varies according to 

$$q(t)=Q_f(1-e^{-t/\tau})$$

where $\tau\equiv RC$, $R$ is the equivalent resistance, and $Q_f$ is the final charge on the capacitor, that is, the charge on the capacitor as $t\rightarrow\infty$ (instead of $t\rightarrow\infty$, it is technically more accurate to say $t\gg \tau$).

To find $Q_f$, replace the capacitor with an open circuit and use Kirchoff's voltage law to find the find the voltage across the capacitor, $V_f$. Then use $Q_f=CV_f$.

## Example

Find $q(t)$ for the following circuit, assuming that the switch is closed at $t=0$.

<img src="figures/Charging_a.svg"/>

**Answer**: When the switch is closed, charge builds up on the capacitor. This build-up continues until the charge on the capacitor is such that no current flows in the circuit. If there is no current flowing through the capacitor, the circuit is equivalent to one in which the capacitor is replaced with an open circuit, as shown below. 

<img src="figures/Charging_b.svg"/>

Kirchhoff's Voltage Law gives

$\mathcal{E}-i(t)R-v_C(t)=0$

For large $t$, $i(t)=0$, so we are left with $v_{C}(t)=\mathcal{E}$. This is a voltage for large $t$, so we relabel it as $V_f$. Using $Q_f=CV_f$ gives $Q_f=C\mathcal{E}$, so

$$q(t)=C\mathcal{E}(1-e^{-t/RC})$$

# Charge/Discharge Problem

## Part I

<img src="figures/Charge_Discharge.svg"/>

The switch in the above circuit has been in position $a$ for a long time. At time $t = 0$ the switch is moved to position $b$. The values of circuit elements are: $\mathcal{E}= 12\text{ V}$, $C = 10\text{ mF}$, and $R = 20\text{ }\Omega$.

Let $t=0^-$ correspond to the time just before the switch is moved from $a$ to $b$. Let $t=0^+$ correspond to the time just after the switch is moved from $a$ to $b$.

1. What is the current through the resistor at $t=0^-$?

   **Answer**: Just before the switch is thrown, the current is zero. By Kirchhoff's loop rule, the voltage across the capacitor, $V_C$, must be equal to the voltage of the power source, so $V_C = \mathcal{E} = 12\text{ V}$.

2. What is the current through the resistor at $t=0^+$?

   **Answer**: Immediately after the switch is moved to $b$, the capacitor starts to discharge though the resistor. By Kirchhoff's loop rule, the voltage across the resistor equals the voltage across the capacitor,  $V_C$. The current through the resistor is $I = V_C/R = 12\text{ V}/20\text{ }\Omega = 0.6\text{ A}$.

3. What is the charge on the capacitor at $t=0^-$?

   **Answer**: Just before the switch is thrown the charge on the capacitor is: $Q = CV_C = (10 \text{ mF})(12\text{ V}) = 120\text{ mC}$.

4. What is the charge on the capacitor at $t=0^+$?

   **Answer**: $120\text{ mC}$

5. What is the charge on the capacitor at $t = 200\text{ ms}$?

   {\bf Answer: } The time constant for the RC circuit is $RC= (10\text{ mF}) (20\text{ }\Omega) = 200\text{ ms}$. At $t = 200\text{ ms}$ after the switch was moved, the capacitor is in the process of discharging. The charge on the capacitor varies according to $q(t)=Q_oe^{-t/RC}$, so

   $q(200\text{ ms}) = Q_0e^{-200\text{ ms}/RC} = 120\text{ mC} \cdot e^{-200\text{ ms}/200\text{ ms}} \simeq120\text{ mC}\cdot 0.37 \simeq 44 \text{ mC}$.

## Part II

<img src="figures/Charge_Discharge.svg"/>

The switch in the above circuit has been in position $b$ for a long time. At time $t = 0$ the switch is moved to position $a$. The values of circuit elements are: $\mathcal{E}= 12\text{ V}$, $C = 10\text{ mF}$, and $R = 20\text{ }\Omega$.

Let $t=0^-$ correspond to the time just before the switch is moved from $a$ to $b$. Let $t=0^+$ correspond to the time just after the switch is moved from $a$ to $b$.

1. What is the current through the resistor at $t=0^-$?

   {\bf Answer: } Since the switch is on position $b$ for a long time, the charge on and voltage across the capacitor is zero. If the voltage across the capacitor is zero, then by Kirchhoff's voltage law the voltage across the resistor must be zero. So the current through the resistor is zero.  

2. What is the charge on the capacitor at $t=0^-$?

   {\bf Answer: } Zero.

3. What is the charge on the capacitor at  $t=0^+$?

   {\bf Answer: } Zero.

4. What is the current through the resistor at $t=0^+$?

   {\bf Answer: } Kirchhoff's voltage law at this time is
   
   $\mathcal{E}-i(0^+)R-v_C(0^+)=0$
   
   At $t=0^+$ the voltage across the capacitor is zero because it is uncharged, so $i(0^+)R=\mathcal{E}$. Thus, the current through the resistor is $i(0^+) = \mathcal{E}/R = 12\text{ V}/20\text{ }\Omega = 0.6\text{ A}$.  

5. What is the charge on the capacitor at time $t = 200\text{ ms}$?

   {\bf Answer: } The time constant is $RC=200\text{ ms}$. At $t=200\text{ ms}$, the charge accumulated on the capacitor is:

   $$q(200\text{ s}) = C\mathcal{E}(1-e^{-(200\text{ s})/RC}) = (10\text{ mF} \cdot 12\text{ V})(1-e^{-200/200})$$
