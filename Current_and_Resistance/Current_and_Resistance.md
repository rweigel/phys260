```mdextension
Title: Current and Resistance
```

# Introduction

## Definitions

The electric current in a wire is defined as 

$$I = \frac{dQ}{dt}$$

where $dQ$ is the total amount of charge that passes through a cross--section of the wire in a differential amount of time, $dt$.

The SI units of $I$ are Coulombs per second, $\text{C}/s$, which is defined to be an Ampere ($\text{A}$).

If $q$ is the charge (in Coulombs) of each flowing charge, $n$ is their number per volume ("number density"), $v_d$ their average speed along the wire (called the "drift speed"), then

$I = n|q|v_dA$, where $A$ is the cross--sectional area of the wire. __Caution__: The $A$ here is itallicized whereas the abbreviation of an Ampere, $\text{A}$ is not itallicized.

The average current density is defined as

$\ds J=\frac{I}{A}$, which can be written as $J = n|q|v_d$.

## Ohm's Law

If an electric field exists in a wire (by, for example, connecting its ends to a battery), the charges will accelerate until they collide with another particle and decelerate (collisions resist the flow). The net result will be current -- a flow of charges with an average drift speed. Experimentally, it has been shown that in many materials, the electric field is proportional to the current density: 

$$E = \rho J$$

where the value of the proportionality constant $\rho$, called resistivity, depends on the material. This is one version of Ohm's law.

For a wire of length $L$ and constant cross--sectional area $A$, Ohm's law can also be written as $V = ({\rho L}/{A}) I$. If we define resistance as $R = {\rho L}/{A}$, then we have another relationship that is also referred to as Ohm's law: 

$V = I R$.

In this form, the interpretation is that the voltage between the ends of a wire is proportional to the current in the wire, with the proportionality constant of $R$.

\newpage

# Problems 

## Definitions and Ohm's Law

A $9$--volt power source is connected to a wire of length $10$ meters with a circular cross--section and radius of $0.01$ meters. The wire has a resistivity of $10^{-8}\text{ }\Omega\cdot\text{m}$. The number density of flowing charges is $10^{28}/\text{m}^3$. Assume Ohm's law applies and the charges that flow are electrons.

1. What is the resistance (with units) of the wire?

    \ifsolutions
    **Answer**: $\ds R=\frac{\rho L}{A} = \frac{(10^{-8}\text{ }\Omega\cdot\text{m})(10\text{ m})}{\pi (0.01\text{ m})^2} = \frac{10^{-3}}{\pi}\text{ }\Omega$. When solving circuit problems, the resistors involved typically have a much larger resistance than this, which is why we neglect the resistance of the wires.
    \else
    \vspace{7em}
    \fi

2. What is the current (with units) in the wire?

    \ifsolutions
    **Answer**: $\ds I = \frac{9\text{ v}}{\frac{10^{-3}}{\pi}\text{ }\Omega}=9,000\pi\text{ C/s} = 9,000\pi\text{ A}$. This is a huge current. If you look at the back of an electronic device, you will see a rating on the order of $1\text{ A}$. Household circuit breakers are set to open ("trip") at approximately $15\text{ A}$. Most power sources cannot supply current at this rate; even if the power source could supply this current, the amount of heat created would lead to a fire or melting of the wire.
    \else
    \vspace{7em}
    \fi

3. How much charge (in Coulombs) flows past a cross--section of the wire per second?

    \ifsolutions
    **Answer**: $9,000\pi\text{ C}$

    Many student are confused by this question, perhaps because it is simple. If current measures the amount of charge that flows past a cross section per unit time, the amount of charge that flows past that cross section in a time of 1 s is the current x 1 s.
    __Caution__: The abbreviation of Coulomb is $\text{C}$ (not itallicized). Later, you will work with capacitance, which we denote with $C$ (itallicized) ... and the unit of capacitance is the Farad ($\text{F}$).
    \else
    \vspace{7em}
    \fi

4. How many electrons flow past a cross--section of the wire per second?  (The charge on an electron is $-1.6·10^{-19}\text{ C}$.)

   Have you ever encountered a number on the order of $10^{23}$ before?

    \ifsolutions
    **Answer**:

     $$9,000\pi\text{ C} \cdot \frac{1\text{ electron}}{1.6\cdot 10^{-19}\text{ C}} \approx 1.8\cdot 10^{23}\text{ electrons}$$

    Avogadro's number, $6.02214076 \times 10^{23}$, is the approximate number of atoms found in 12 grams of pure carbon-12. A mol is used to describe exactly $6.02214076 \cdot 10^{23}$ items (such as atoms, molecules, ions, or electrons).
    \else
    \vspace{7em}
    \fi


5. What is the current density (with units)?

    \ifsolutions
    **Answer**: $\ds J=\frac{I}{A} = 9\cdot 10^7 \frac{\text{A}}{\text{m}^2}$ (note the $A$ in the first equation is a cross-sectional aread and the $\text{A}$ in the second equation corresponds to an Ampere).
    \else
    \vspace{7em}
    \fi

6. What is the drift velocity of electrons in the wire? (The charge on an electron is $-1.6·10^{-19}\text{ C}$.)

    \ifsolutions
    **Answer**: $v_d = J/n|q| \simeq 6\text{ cm/s}$
    \else
    \vspace{7em}
    \fi

7. Based on the description of how charged particles flow in a wire, explain why the resistance of a cylindrical wire is proportional to its length and inversely proportional to the square of its radius.

    \ifsolutions
    **Answer**: See the description in your textbook.
    \else
    \fi

\ifsolutions
\else
\newpage
\fi

## Definitions and Ohm's Law
 
A power source is connected to a $20$ meter long wire with a circular cross--section and radius of $0.01$ meters. The wire has a resistivity of $10^{-7}\text{ }\Omega\cdot\text{m}$. The number density of flowing charges is $10^{27}/\text{m}^3$. The current in the wire was measured and found to be $1\text{ A}$. Assume Ohm's law applies and the charges that flow are electrons.

1. What is the resistance (with units) of the wire?

    \ifsolutions
    **Answer**: $(.02/\pi)\text{ }\Omega$
    \else
    \vspace{7em}
    \fi

2. How much charge (with units) flows past a cross--section of the wire per second?

    \ifsolutions
    **Answer**: $1\text{ C}$
    \else
    \vspace{7em}
    \fi

3. What is the current density (with units)?

    \ifsolutions
    **Answer**: $\ds J = \frac{10^4}{\pi}\frac{\text{A}}{\text{m}^2}$
    \else
    \vspace{7em}
    \fi

4. What is the drift velocity of electrons in the wire? (The charge on an electron is $-1.6·10^{-19}\text{ C}$.)

    \ifsolutions
    **Answer**: $v_d = J/n|q| = 0.02\text{ mm/s}$
    \else
    \vspace{7em}
    \fi

\ifsolutions
\else
\newpage
\fi

## Current Through a Cylindrical Shell

If a cylindrical wire with an inner radius $a$ and outer radius $b$ carries a current $I$, what is $J$?

\ifsolutions
**Answer**: $\ds J=\frac{I}{\pi(b^2-a^2)}$
\else
\vspace{7em}
\fi

## $I = n|q|v_dA$ derivation

Derive the relationship $I = n|q|v_dA$. Provide a diagram.

\ifsolutions
**Answer**: See textbook.
\else
\fi
