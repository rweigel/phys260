```mdextension
Title: Equivalent Resistance
```

# Introduction

The current in all parts of a circuit with resistors and batteries can always be found by writing equations for KCL and KVL and solving for the unknown currents. This was the approach taken in the Kirchhoff's law activity.

There is an alternative approach that is often faster:

1. replace resistors in series or parallel with equivalent resistances to create a new circuit. If no resistors in the new circuit are in series or parallel, skip to step 3.
2. repeat step 1.
3. Use KCL and KVL to find currents in the remaining equivalent circuit.

In many problems, we are only interested in the currents through the batteries, so no further analysis is needed beyond step 3. If the currents in the resistors of the original circuit are needed, rebuild it step--by--step, finding all currents at each step using KCL and KVL.

# Single Loop

Reduce the following circuit as much as possible using equivalent resistances. Then, find $I$.

<img src="figures/Series.svg" height="130px">

\ifsolutions
**Answer**: $I = \mathcal{E}/R_{\text{eq}}$, where $R_{\text{eq}}=R_1+R_2$

<img src="figures/Series_Equivalent.svg" height="100px">

\else
\fi

# Multiple Loops I

Reduce the following circuit as much as possible using equivalent resistances. Then find $I_o$.

<img src="figures/Parallel.svg" height="200px">

\ifsolutions
**Answer**: $I_o=\mathcal{E}/R_{\text{eq}}$, $R_{\text{eq}}=\frac{1}{\left(\frac{1}{R_1}+\frac{1}{R_2}\right)}$.

<img src="figures/Parallel_Equivalent.svg" height="100px">
\else
\fi

# Multiple Loops II

Reduce the following circuit as much as possible using equivalent resistances. Then find $I_1$.

<img src="../Kirchhoffs_Laws/figures/Multiple_Loops_I_No_Annotation.svg" height="200px">

\ifsolutions
**Answer**: 

The two lower resistors are in parallel and can be replaced with a resistor having an equivalent resistance of 

$$R_{\text{eq}}=\frac{1}{\frac{1}{R} + \frac{1}{R}} = \frac{R}{2}$$

The new circuit is

<img src="figures/Multiple_II_Equivalent_1.svg" height="100px">

In the above circuit, the two resistors are in series and can be replaced with a resistor having an equivalent resistance of

$$R_{\text{eq}} = R+\frac{R}{2} = \frac{3}{2}R$$

<img src="figures/Multiple_II_Equivalent_2.svg" height="100px">

$I_1=\mathcal{E}/R_{\text{eq}}$, where $R_{\text{eq}}=3R/2$; This is the same answer that was found for the identical circuit in the Kirchhoff's law activity by solving three equations.

\else
\vspace{10em}
\fi

# Multiple Loops III

Reduce the following circuit as much as possible using equivalent resistances. Then find the equations for KCL and KVL that are needed to find the currents through $\mathcal{E}_o$ and $\mathcal{E}_1$.

<img src="figures/Two_Batteries.svg" height="150px">

\ifsolutions
**Partial Answer**:

The two outer resistors are in parallel and can be replaced with a resistor having an equivalent resistance of $R/2$.

<img src="figures/Two_Batteries_Equivalent.svg" height="150px">

No further reduction is possible. At this point, we must use KCL and KVL to find the currents.

<img src="figures/Two_Batteries_Equivalent_With_Annotation.svg" height="150px">

The currents can be found by solving

$I_o+I_1 = I_2$

$-I_or + \mathcal{E}_o - \mathcal{E}_1 + I_1r = 0$

$-I_1r + \mathcal{E}_1 - I_2(R/2) = 0$

\else
\newpage
\fi

# Rebuilding I

Find all of the currents in the circuit in Multiple Loops I.

\ifsolutions

The original circuit was:

<img src="figures/Parallel.svg" height="200px">

We know the voltage across each resistor is $\mathcal{E}$, so we can write $I_1=\mathcal{E}/R_1$ and $I_2=\mathcal{E}/R_2$.

Check: $I_1+I_2=I_o$ is satisfied because we found $I_o=\mathcal{E}/R_{\text{eq}}$, where $R_{\text{eq}}=\frac{1}{\left(\frac{1}{R_1}+\frac{1}{R_2}\right)}$, so 

$I_o=\mathcal{E}\left(\frac{1}{R_1}+\frac{1}{R_2}\right)$.

\else
\vspace{20em}
\fi

# Rebuilding II

Find all of the currents in the circuit in Multiple Loops II.

\ifsolutions
**Answer**:

In the following circuit, we know $I_1$, so the voltage drop across the lower resistor is $I_1R/2$.

<img src="figures/Multiple_II_Equivalent_1.svg" height="100px">

This voltage, $I_1R/2$, is also the voltage across the two lower resistors in the original circuit shown below.

<img src="../Kirchhoffs_Laws/figures/Multiple_Loops_I_No_Annotation.svg" height="200px">

So $I_2=(I_1R/2)/R=I_1/2$ and $I_3=(I_1R/2)/R=I_1/2$ (Note that the $I_2=I_3$ is expected.)

Check: $I_2+I_3=I_1$

\else
\newpage
\fi

# Rebuilding III

Find all of the currents in the circuit in Multiple Loops III.

\ifsolutions
**Partial Solution**: Once $I_1$ is known, so is the voltage across the two outer resistors: $\mathcal{E}_1-I_1r$. So the current in the outer resistors, which have the same resistance $R$, will be $(\mathcal{E}_1-I_1r)/R$.
\else
\vspace{10em}
\fi
