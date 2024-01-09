```mdextension
Title: Sound Intensity Level
```

# Introduction

The intensity of a sound wave, $I$, is the average power rate per unit area of energy from a sound wave that passes through or into a surface,

$$I = \frac{P}{A}$$

$I$ has units of Power/Area, which has SI units of $\text{Watts}/\text{m}^2$. The intensity of various sources of sound is shown in the third column of the following table from Young and Freedman, 14th Edition. The second column is discussed in section 3 of this activity.

<img src="figures/Table16.2.png" width=50%/>

If the sound wave is created by a point source with power $P$, is emitted uniformly in all direction (isotropically), and there are no reflections or obstructions, the intensity varies with the distance $r$ from the point source according to

$$I = \frac{P}{4\pi r^2}$$

Because $I$ is proportional to $r^2$, if the disance from the source doubles, the intensity decreases by a factor of four.

\newpage

# Sound Intensity, $I$

Suppose a bird sitting on the top of a lamp post emits sound with a power of $1\text{ W}$; assume that the relationship $I = P/4\pi r^2$ applies.

1. What is $I$ at a point $5\text{ m}$ away?

   \ifsolutions
   **Answer**:

   $$I = \frac{1\text{ W}}{4\pi (5\text{ m})^2} \simeq \frac{1}{314} \frac{\text{ W}\phantom{^2}}{\text{m}^2}$$
   \else
   \vspace{10em}
   \fi

2. What is $I$ at a point $50\text{ m}$ away?

   \ifsolutions
   **Answer**: If the distance increases by a factor of $10$, we expect $I$ to descrease a factor of $100$ (because $I$ is inversely proportional to area and area depends on the square of the distance). So

   $$I = \frac{1}{3140} \frac{\text{ W}\phantom{^2}}{\text{m}^2}$$

   \else
   \vspace{10em}
   \fi

----

A siren is emitting sound at a constant intensity level; assume assume that the relationship $I = P/4\pi r^2$ applies.

3. If you move three times farther away from the siren, by what ratio does the sound intensity change?

   \ifsolutions
   **Answer**:

   Because intensity is proportional to $1/r^2$, moving 3 time farther away will decrease the intensity by a factor of $1/9$. This can be shown in more detail by noting that $I_1 = P_1/A_1$, $I_2=P_2/A_2$ and the power is constant, so $P_1=P_2$. Thus,
   
   $$\frac{I_2}{I_1} = \frac{A_1}{A_1} = \frac{4\pi d_1^2}{4\pi d_2^2} =  \frac{d_1^2}{d_2^2}$$

   If $I_1$ is your initial position at $d_1$, then $d_2 = 3d_1$ and

   $$\frac{I_2}{I_1} =  \frac{d_1^2}{d_2^2} = \frac{d_1^2}{(3d_1)^2} = \frac{1}{9}$$

   So decreases by a factor of $9$.

   \else
   \vspace{10em}
   \fi

4. If instead you moved four times closer to the siren, by what ratio does the sound intensity change?

   \ifsolutions
   **Answer**: Increases by a factor of $16$.
   
   $$\frac{I_2}{I_1} = \frac{d_1^2}{d_2^2} =  \frac{d_1^2}{(d_1/4)^2} = 16$$
   \else
   %\vspace{10em}
   \fi

\newpage

# Sound Intensity Level, $\beta$

Because of the sound intensity values of human hearing span a very large range, from $0.0000000000001$ to $100$ $\text{Watts}/\text{m}^2$ (see the table in the introduction), we define an alternative measure of intensity called the sound intensity _level_, $\beta$. The equation that relates sound intensity level $I$, with sound intensity, $\beta$, is

$$\beta = (10 \text{ dB})\log_{10}\left(\frac{I}{I_o}\right)$$

where $\text{dB}$ stands for "decibels".

One advantage to using this formula is that its values span a much smaller range, from 0--140, as shown in the second column of the table in the introduction. Another advantage is that the reference value of zero corresponds to something easily interpreted: $0\text{ dB}$ means something that is barely audible by humans.

1. Logarithmic scales are often used in science an engineering. Give at least one other example besides sound intensity level that is a quantity that is based on a logarithmic scale.

   \ifsolutions
   **Answer**: pH scale for acidity, Richter earthquake magnitude scale.
   \else
   \vspace{8em}
   \fi

2. If you increase the sound intensity of a speaker on a TV from $I_1$ to $I_2$ and $I_2/I_1=10$, what is $\beta_2-\beta_1$?

   \ifsolutions
   In the table, each factor of $10$ increase in $I$ corresponds to an change in $\beta$ by $+10$. So $\beta_2-\beta_1 = 10\text{ dB}$. We can also use

   $$\beta_1 = (10 \text{ dB})\log_{10}\left(\frac{I_1}{I_o}\right)$$

   $$\beta_2 = (10 \text{ dB})\log_{10}\left(\frac{I_2}{I_o}\right)$$

   $$\beta_2-\beta_1 = (10 \text{ dB})\left[\log_{10}\left(\frac{I_2}{I_o}\right)-\log_{10}\left(\frac{I_1}{I_o}\right)\right]$$

   Using $\log_{10}y - \log_{10}x = \log_{10}(y/x)$ gives

   $$\beta_2-\beta_1 = (10 \text{ dB})\left[\log_{10}\left(\frac{I_2}{I_1}\right)\right]$$
   
   So if $I_2/I_1 = 10$, we have

   $$\beta_2-\beta_1 = (10 \text{ dB})\left[\log_{10}(10)\right]= 10 \text{ dB}$$

   \else
   \vspace{8em}
   \fi

3. If you increase the sound intensity level of a speaker on a TV from $\beta_1$ to $\beta_2$ and $\beta_2-\beta_1=20\text{ dB}$, what is $I_2/I_1$?

   **Answer**: 
   
   $$20\text{ dB} = (10 \text{ dB})\left[\log_{10}\left(\frac{I_2}{I_1}\right)\right]$$

   Dividing both sides by $10 \text{ dB}$ gives
   
   $$2 = \log_{10}\left(\frac{I_2}{I_1}\right)$$
   
   Raising both sides by $10$ and using the identity $10^{\log_{10}x} = x$ gives

   $$10^2 = \frac{I_2}{I_1}$$

   This could also have been determined using the table in the introduction. The difference in $\beta$ for a whisper ($20\text{ dB}$) to $\beta$ for the threshold of hearing ($0\text{ dB}$) is $20\text{ dB}$. The ratio of $I$ for a whisper ($10^{-10}\text{ W}/\text{m}^2$) to $I$ for the threshold of hearing ($10^{-12}\text{ W}/\text{m}^2$) is $10^{-10}/10^{-12}=100$.
   \ifsolutions
   \else
   \vspace{6em}
   \fi

----

4. A city council adopted a law to reduce the maximum allowed sound intensity level of leaf blowers from $95\text{ dB}$ to $70\text{ dB}$. With the new law, what is the ratio of the new maximum allowed intensity to the previously allowed intensity?

   \ifsolutions
   **Answer**:

   From the solution to problem 3.2,

   $$\beta_2-\beta_1 = (10 \text{ dB})\left[\log_{10}\left(\frac{I_2}{I_1}\right)\right]$$

   If $\beta_2$ corresponds to the new maximum sound intensity level and $\beta_1$ the old,

   $$(70-95)\text{ dB} =  (10 \text{ dB})\log_{10}\left(\frac{I_2}{I_1}\right)$$

   $$-2.5 = \left(\frac{I_2}{I_1}\right)$$
   
   $$10^{-2.5} = \frac{I_2}{I_1}$$

   $$\frac{I_2}{I_1} = \frac{1}{10^{2.5}} \simeq \frac{1}{316}$$

   \else
   \vspace{8em}
   \fi

----

A siren is emitting sound at a constant intensity level

5. If you move three times closer to the siren, what is the change in the sound intensity level?

   \ifsolutions
   \else
   \vspace{8em}
   \fi

6. If instead you moved four times closer to the siren,, what is the change in the sound intensity level ?

   \ifsolutions
   \else
   \vspace{8em}
   \fi

----

7. You are trying to hear a juicy conversation, but from your distance of 15.0 m it sounds like only an average whisper of 20.0 dB. How close should you move to the chatterboxes for the sound level to be 60.0 dB? Show your work.

   \ifsolutions
   From the solution to problem 3.2,

   $$\beta_2-\beta_1 = (10 \text{ dB})\left[\log_{10}\left(\frac{I_2}{I_1}\right)\right]$$

   From the solution to problem 2.2,
   
   $$\frac{I_2}{I_1} = \frac{d_1^2}{d_2^2}$$

   \else
   \vspace{8em}
   \fi

8. Solve for $I$ in the equation $\beta = (10 \text{ dB})\log_{10}\left(\frac{I}{I_o}\right)$

   \ifsolutions
   **Answer**:
   
   Divide both sides by ${10 \text{ dB}}$

   $$\beta/(10 \text{ dB})  = \log_{10}\left(\frac{I}{I_o}\right)$$

   Raising both sides to the power of $10$ gives

   $$10^{\beta/(10 \text{ dB})} = 10^{\log_{10}\left(\frac{I}{I_o}\right)}$$

   Using the identity $10^{\log_{10}x} = x$,

   $$10^{\beta/(10 \text{ dB})} = \frac{I}{I_o}$$

   Solving for $I$ gives   

   $I=I_o 10^{\beta/(10\text{ dB})}$
   \else
   \vspace{8em}
   \fi

8. Solve for $I_2/I_1$ in the equation $\beta_2-\beta_1 = (10 \text{ dB})\log_{10}\left(\frac{I_2}{I_1}\right)$

   \ifsolutions
   **Answer**:

   $$\frac{I_2}{I_1}=10^{(\beta_2-\beta_1)/(10\text{ dB})}$$

   \else
   \vspace{8em}
   \fi