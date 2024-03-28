```mdextension
Title: LRC and AC Circuits
```

# Introduction

Previously, we have examined circuits that are powered by batteries which produce constant voltage (called a direct current, or DC). However, our power distribution system makes use of alternating current (AC) in which the voltages and currents vary sinusoidally with time. 

## R Only

The following figure shows a circuit in which an AC power source causes the current to vary  sinusoidally in time according to $i(t)=I\cos(\omega t)$. By Ohm's law, the equation for the instantaneous voltage across the resistor is $v_R(t) = IR\cos(\omega t)$.

\include{RLC and AC Circuits/figures/31_07_FigureA.jpg}
\include{RLC and AC Circuits/figures/31_07_FigureB.jpg}

We say that the voltage and current are "in phase" because the peaks, valleys, and zero crossings in the plots of $i(t)$ and $v_R(t)$ occur at the same time. 

## L Only

As before, the following figure shows a circuit in which an AC power source causes the current to vary sinusoidally in time according to $i(t)=I\cos(\omega t)$. 

In this case, the voltage across the inductor varies according to $v_L(t) = I\omega L\cos(\omega t + 90^o)$.

Because the term $\omega L$ occurs frequently, we give it a name of {\bf inductive reactance}: $X_L \equiv \omega L$. With this new variable, $v_L(t) = IX_L\cos(\omega t + 90^\circ)$.

We say the voltage across the inductor "leads" the current by $90^\circ$ (or, equivalently, $T/4$) because the maxima (or minima) in $v_R(t)$ occur before the maxima (or minima) in $i(t)$. In the following figure, the first minima of the plot of $v_R(t)$ is shown to occur earlier than the first minima in the $i(t)$ plot by $T/4$ (or equivalently, by $90^\circ$ or $\pi/2$).

\include{RLC and AC Circuits/figures/31_08_FigureA.jpg}

\include{RLC and AC Circuits/figures/31_08_FigureB.jpg}

## C Only

As before, the following figure shows a circuit in which an AC power source causes the current to vary sinusoidally in time according to $i(t)=I\cos(\omega t)$. 

In this case, the voltage across the capacitor varies according to $v_C(t) = (I/(\omega C))\cos(\omega t - 90^o)$.

Because the term $1/(\omega C)$ occurs frequently, we give it a name of {\bf capacitive reactance}: $X_C \equiv 1/(\omega C)$. With this new variable, $v_C(t) = IX_C\cos(\omega t - 90^\circ)$.

We say the voltage across the capacitor "lags" the current by $90^\circ$ (or, equivalently, $T/4$) because the maxima (or minima) in $v_C(t)$ occur after the maxima (or minima) in $i(t)$. In the following figure, the first minima of the $v_C(t)$ is shown to occur after than the first minima in the $i(t)$ plot by $T/4$.

\include{RLC and AC Circuits/figures/31_09_FigureA.jpg}

\include{RLC and AC Circuits/figures/31_09_FigureB.jpg}

## Series LRC circuit

Suppose that we know the current $i(t)$ in the following series LRC circuit is $i(t)=I\cos(\omega t)$.

\includegraphics[scale=0.3]{RLC and AC Circuits/figures/31_13_FigureA.jpg}

We want to know the voltage across the AC power supply, $v_{d}-v_{a}$, which we call $v$.

We know the voltage across each of the components from the discussion above.

$$
v_R(t) = IR\cos(\omega t)
$$

$$
v_L(t) = I\omega L\cos(\omega t + 90^\circ) = IX_L\cos(\omega t + 90^\circ)
$$

$$
v_C(t) = (I/(\omega C))\cos(\omega t - 90^\circ)=IX_C\cos(\omega t - 90^\circ)
$$

From Ohm's law, the voltages around a loop must be zero. From this, we have

$$
v(t)=v_R(t)+v_L(t)+v_C(t)
$$

Substitution gives

$$
v(t)=IR\cos(\omega t)+IX_L\cos(\omega t + 90^\circ)+IX_C\cos(\omega t - 90^\circ)
$$

In this activity, you will compute $v(t)$ in two ways. First, you will use the above formula and a trig identity to write $v(t)$ in the form $IZ\cos(\omega t+\phi)$, where the constants $Z$ and $\phi$ depend on $R$, $L$, and $C$ (or equivalently, $R$, $X_L$, and $X_C$). Next, you will use a general formula to compute $Z$ and $\phi$.

## Problem

Suppose you have a LRC circuit where $I$, $R$, $L$, and $C$ are given such that $IR=1\text{ [V]}$, $IX_L=1\text{ [V]}$, and $X_C=0$. In addition, we are given $i(t)=(1\text{ [A]})\cos\omega t$ and $\omega = 2\pi\text{ }[\text{s}^{-1}]$.

On the {\bf same} graph,

1.  Compute the period, $T$, of $i(t)$

    {\bf Answer}: There are two ways to answer this. (1) The current is $i(t)=\cos\omega t$. At $t=0$, $i=1$. When $\omega t=2\pi$, $i=1$ again for the first time. So the time for the $i(t)$ to be where it started is $t$ such that $\omega t=2\pi \Rightarrow t = 2\pi/(2\pi~[\text{s}^{-1}])=1~\text{ s}$. (2) Remember the formula $T=2\pi/\omega$.

2.  Plot $i(t)$

    {\bf Answer}: See https://www.desmos.com/calculator/klkajsstdc

3.  Plot $v_R(t)$

    {\bf Answer}: See Desmos plot

4.  Plot $v_L(t)$

    {\bf Answer}: See Desmos plot

5.  Plot $v_C(t)$

    {\bf Answer}: See Desmos plot. Note that $v_C = 0$ when $X_C=1/(\omega C)=0$. To get $X_C\approx 0$ in the Desmos plot, we set $C=1000$.

6.  Starting with $v(t)=v_R(t)+v_L(t)+v_C(t)$, use a trig identity to write $v(t)$ in the form\\ $v(t)=Z\cos(\omega t + \phi)$. That is, find the constants $Z$ and $\phi$. The trig identity is\\ $A\cos(\theta) + B\cos(\theta + \pi/2)=\sqrt{A^2+B^2}\cos\left(\theta + \tan^{-1}(B/A)\right)$

    {\bf Answer}: Here we have $v_R(t)=\cos\omega t$, $v_L(t)=\cos(\omega t+\pi/2)$, and $v_C(t)=0$, so $v(t)=\cos\omega t+\cos(\omega t+\pi/2)$. Comparing this with the identity, $A=B=1$ and we get $v(t)=\sqrt{2}\cos(\omega t + \tan^{-1}(1/1))=\sqrt{2}\cos(\omega t+\pi/4)$. Because of the $+\pi/4$, we say that $v(t)$ leads $i(t)$ by $\pi/4$ (or $45^\circ$ or $T/8$).

7.  Plot $v(t)$

    {\bf Answer}: See Desmos plot. Try to adjust the parameters $R$, $L$, and $C$ to see how they change the curves (both amplitudes and phases).

## Problem

In the previous problem, computing $v(t)$ required the use of a trig identity to combine $v_R$ and $v_L$ and write $v(t)$ in the form $v(t)=Z\cos(\omega t + \phi)$, where $Z$ and $\phi$ are constants that depend on $L$ and $R$. When $v_C$ is not zero, additional algebra is needed to compute $v(t)$ (by using the trig identity again). However, there is formula that can be used to find $v(t)$ in general so that trig identities are not needed to compute $v(t)$.

It can be shown that in general, the voltage across the AC power source is

$$
v(t) = IZ\cos(\omega t + \phi)
$$

Where the series LRC {\bf impedance} $Z$ is defined as

$$
Z = \sqrt{R^2 + (X_L-X_C)^2}
$$

and the {\bf phase angle} $\phi$ of $v(t)$ is defined as

$$
\phi = \tan^{-1}\left(\frac{X_L - X_C}{R}\right) = \tan^{-1}\left(\frac{\omega L - 1/(\omega C)}{R}\right)
$$

When $\phi$ is positive, $v(t)$ leads $i(t)$. When $\phi$ is negative, $v(t)$ lags $i(t)$. When $\phi=0$, $v(t)$ is in phase with $i(t)$.

1.  Using the parameters given in the previous problem, find $v(t)$ using the above formula.

    {\bf Answer}: In the previous problem, we were given $I=1$ and $\omega=2\pi$, $IR=1$, $IX_L=I\omega L=1$, $X_C=1/(\omega C)$. From this, we conclude $R=1$, $\omega L=1$, and $1/(\omega C)=0$. Thus

    $$
    Z = \sqrt{R^2 + (X_L-X_C)^2} = \sqrt{1^2 + (1 - 0)^2}
    $$

    and

    $$
    \phi = \tan^{-1}\left(\frac{X_L - X_C}{R}\right) = \tan^{-1}\left(\frac{1-0}{1}\right)=\tan^{-1}\left(\frac{1}{1}\right) = \frac{\pi}{4}
    $$

    Thus,

    $$
    v(t) = IZ\cos(\omega t + \phi) = \sqrt{2}\cos(\omega t+\pi/4)
    $$

    which is the same as found in the previous problem.

2.  Does $v(t)$ lead or lag $i(t)$?

    {\bf Answer}: Lead. A plot of $i(t)$ and $v(t)$ shows that peaks in $v(t)$ occur {\it before} peaks in $i(t)$.