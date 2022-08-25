# LR Circuits (Ch 30)

## Introduction

\input{LR/figures/lr}

The above figure shows a LR series circuit consisting of an inductor of inductance $L$ connected in series with a resistor of resistance $R$. The switch, $S$, is closed at a time $t = 0$ and then remains closed. 

Using Kirchhoff’s voltage law around the loop, we have

$$
V_s - I(t) \cdot R - L \frac{dI(t)}{dt} = 0
$$

The term $L dI/dt$ is called the induced emf.

The above differential equation can be solved for $I(t)$, the current at any time given the initial value of $I$, which is zero. The result is

$$
I(t)=\frac{V_s}{R}\left(1-e^{-t/(L/R)}\right)
$$

After a long time, the current approaches a constant value of $I = V_s/R$ because the exponential term approaches zero and so there is effectively no time dependence in $I(t)$. How quickly the exponential term approaches zero depends on a quantity called the LR time constant defined by

$$\tau = L/R$$

which has units of seconds when $L$ is in Henrys and $R$ is in Ohms. With this, we can write

$$
I(t) = \frac{V_s}{R}\left(1-e^{-t/\tau}\right)
$$

In this equation, at $t=0$, the current is

$$
I(0) = (V_s/R)\left(1-e^{-0/\tau}\right)=(V_s/R)\left(1-1\right)=0
$$

As a result, we state that initially the inductor behaves like an open circuit because current does not flow though it.

For large $t/\tau$, the exponential term becomes much smaller than one and so the current becomes a constant value of $V_s/R$. If we replace the inductor with a wire, this is the same current that we would find. As a result, we state that after a long time, the inductor behaves like a resistanceless wire.

## Problem

\input{LR/figures/lr_plot}

In this problem, you will consider the equation

$$I(t) = \frac{V_s}{R}\left(1-e^{-t/\tau}\right)$$

that was described in the introduction.

* If $V_s/R=10\text{ A}$, plot dots for the values of $I$ at $t=0, 2, 4, 6, 12\text{ s}$ with $L/R = \tau = 2\text{ s}$ 
    
* Based on the equation, at $t=0$ does an inductor behave like an open circuit or a wire?
    
    {\bf Answer}: At $t=0$ the current will be $0$ with the inductor acting like a break in the circuit with no current flowing.

* Based on the equation, at $t\gg \tau$ does an inductor behave like an open circuit or a wire?

    \bf Answer}: At $t \gg \tau$ the current will be $V_s/R$ with the inductor acting like a wire -- the circuit behaves as it would if there were no inductor in it.
    
* If $L$ doubles but $R$ remains constant
    
    a. does the time constant $\tau$ increase, decrease, or remain the same?;
    
    b. how will the points that you drew for part 1. change? (Will they move up, down, or remain the same?) 

    c. Does your answer to b. make sense physically? That is, an inductor tends to impede changes in current and so is your answer to b. consistent with this? 

    {\bf Answer}: If $L$ increases, the inductor provides more resistance to change from its initial state, which is $I=0$. Thus we expect the current to take longer to reach its final state. All of the points (except for $t=0$ will move downward).

* The voltage across the inductor is $LdI/dt$. Compute $dI/dt$ and sketch its curve on the graph above. Is this equation consistent with the statement that for large $t/\tau$, the voltage across the inductor is zero?
    
    {\bf Answer:} $LdI/dt = -V_se^{-t/\tau}$. Yes. The voltage across the inductor is $-V_se^{-t/\tau}$ and for large $t/\tau$, $e^{-t/\tau}$ is near zero.

## Problem

An inductor with an inductance of $40\text{ mH}$ and a resistor with a resistance of 2\Omega$ are connected together to form a LR series circuit. If they are connected to a $20\text{ V}$ DC supply,

*   What will be the final steady state value of the current (the current after a very long time)?

    {\bf Answer}: At the steady state, the current passing through the inductor is constant, the induced emf becomes 0. Consequently, the voltage drop on the resistor is the same as the total voltage of the DC supply. 

    $$
    I = V_s/R=(20\text{ V})/(2\Omega) = 10\text{ A}
    $$

*   What is the time constant of the RL series circuit?

    {\bf Answer}: The time constant is given by $\tau = L/R = (40\text{ mH}w)/(2\Omega) = 20 \text{ ms}$

*   How long does it takes for the current to reach 63\% of its maximum value?

    {\bf Answer}: The current in the circuit is expressed as:

    $$
    I(t)=  \frac{V_s}{R}\left(1-e^{-t/(L/R)}\right)
    $$

    The maximum current value is $I_0=V_s/R$. Therefore, 

    $$
    \frac{I(t)}{I_0} = 1-e^{-t/(L/R)} = 1-e^{-t/\tau} 
    $$

    When $I(t)/I_0 =0.63$ and $\tau = L/R = 40\text{ ms}$:

    $$0.63 = 1-e^{-t/\tau}\Rightarrow\quad e^{-t/\tau} = 1-0.63 = 0.37$$

    $$-t/\tau = \ln(0.37) = -0.9943\quad\Rightarrow\quad t = 19.89\text{ ms}$$

    It takes roughly $20\text{ ms}$ ($\simeq \tau$) to reach $63\%$ of the maximum current value. (So $0.63$ is a special number for an LR circuit -- at $t=\tau$, the current is $0.63$ of its maximum value.)

* What will be the value of the induced emf after $10\text{ ms}$?

    {\bf Answer}: After 10 ms, the current is calculated as:

    $$
    I(t) = \frac{V_s}{R}(1-e^{-t/(L/R)}) = \frac{20 \text{ V}}{2~\Omega} \left(1-e^{-(10\text{ ms})/(20\text{ ms})}\right) = 3.9\text{ A} 
    $$

    The induced emf is:
    $$
    emf = V_s - IR= 20\text{ V} - 3.9\text{ A} \cdot 2~\Omega=12.2\text{ V} 
    $$

* What will be the value of the circuit current one time constant (that is, at $t=\tau$) after the switch is closed?

    {\bf Answer}: At time $t = \tau$,

    $$
    I(t) =  \frac{V_s}{R} (1-e^{-t/\tau})=10 \times (1-0.368) = 6.32\text{ A}
    $$

    This question is related to question 3. In the answer to question 3., it was found that it takes approximately one time constant to reach $63\%$ of the maximum value. So in this problem we expect that the answer to be approximately $63\%$ of the final value.

## Problem

\input{LR/figures/lr_discharge}

In the circuit above, an inductor with $L=10\text{ mH}$ and a resistor with $R=1\Omega$ is connected as shown. The battery has an emf of $10\text{ V}. At $t=0$, the switch $S_1$ is closed.


1.  What is the current through the resistor at $t=0$?

    {\bf Answer}: Zero. There is no closed path for current to flow.

2.  What is the current through the inductor at $t=0$?

    {\bf Answer}: Zero. There is no closed path for current to flow.

3.  After a long time, what will the current be through the resistor and inductor?

    {\bf Answer}: The current in the circuit as a function of time is

    $$
    I(t)=  \frac{V_s}{R}\left(1-e^{-t/(L/R)}\right)
    $$

    For large $t$, the exponential term is near zero, leaving $V_s/R=$10~V/1 $\Omega$ = $10$~A.

4.  After a long time, switch $S_1$ is opened and $S_2$ is closed simultaneously. Write Kirchhoff's voltage law around the new closed loop.

    {\bf Answer}: 
    $$
    - I(t) R - L\frac{dI(t)}{dt} = 0
    $$

5.  Show that the equation $I(t)=(10\text{ A})e^{-t/\tau}$ satisfies the equation in your answer to the previous question.

    {\bf Answer}: Starting with

    $$
    - I(t) \cdot R - L \frac{dI(t)}{dt} = 0
    $$

    And using $I=10e^{-t/\tau}$ and $d e^{t/\tau}/dt=(1/\tau) e^{-t/\tau}$, we have

    $$
    - (10\text{ A})e^{-t/\tau} \cdot (1\Omega) - (10\text{ mH}/\tau)e^{-t/\tau} = 0

    $$
    Using $\tau = L/R$ one arrives at

    $$
    - (10\text{ V})e^{-t/\tau} - (10\text{ V})e^{-t/\tau} = 0
    $$

6.  Plot $I(t)$ from $t=0$ to $t=0.01$~s. Assume that the switch $S_1$ was opened and switch $S_2$ was closed at $t=0.005$~s.
    
    \input{LR/figures/lr_plot}  
