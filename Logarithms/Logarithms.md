```mdextension
Title: Logarithms
```

# Introduction -- Base $10$ Logarithms

The motivation for the base 10 logarithm is that it reduces numbers raised by a power of 10 to the power the number was raised to. So $10^2$ becomes $2$, $10^3$ becomes $3$, etc. The base 10 logarithm is sometimes called the "common logarithm".

In mathematical notation,

$\log_{10}(10^x) = x$

For example, $\log_{10}(10^{-5}) = -5$ and $\log_{10}(10^7) = 7$

(To take the base 10 logarithm of a number that is not exactly a power of $10$, use a calculator.)

Several identities follow as a result:

1. If you raise a base 10 logged number by $10$, you get back the number that was logged.

   $10^{\log_{10}(x)} = x$
   
   For example,
   
   $10^{\log_{10}(7)} = 7$ and  $10^{\log_{10}(8.8)} = 8.8$

2. The sum of two logged numbers is the log of the product of the numbers:

   $\log_{10}y + \log_{10}x = \log_{10}(yx)$;

   For example,

   $\log_{10}10 + \log_{10}100 = \log_{10}10\cdot 100 = \log_{10}10^3 = 3$

3. The difference between two logged number is the log of the ratio of the numbers:
 
   $\log_{10}y - \log_{10}x = \log_{10}(y/x)$

   For example,
   
   $\log_{10}10 - \log_{10}100 = \log_{10}(10/100) = \log_{10}10^{-1} = -1$

## Problems

1. What is $\log_{10}(0.000000001)$?

   \ifsolutions
   **Answer**: $\log_{10}(0.000000001)=\log_{10}(10^{-9})=-9$
   \else
   \vspace{2em}
   \fi

2. What is $\log_{10}(10,000)$?

   \ifsolutions
   **Answer**: $\log_{10}(10,000)=\log_{10}(10^{4})=4$
   \else
   \vspace{2em}
   \fi

3. $\log_{10}(10,000)+\log_{10}(0.000000001)=\log_{10}(x)$. Find $x$.

   \ifsolutions
   **Answer**: $\log_{10}(10^{4}) + \log_{10}(10^{-9}) = \log_{10}(10^{4}\cdot 10^{-9}) = \log_{10}(10^{-5})\Rightarrow x = 10^{-9}$

   \else
   \vspace{2em}
   \fi

3.  $\log_{10}(10,000)-\log_{10}(0.000000001)=\log_{10}(x)$. Find $x$.

   \ifsolutions
   **Answer**: $\log_{10}(10^{4}) - \log_{10}(10^{-9}) = \log_{10}(10^{4}/10^{-9}) = \log_{10}(10^{13})\Rightarrow x = 10^{13}$
   \else
   \vspace{2em}
   \fi

5. If $x = x_o\log_{10}(y/y_o)$, solve for $y$.

   \ifsolutions
   **Answer**: $x/x_o = \log_{10}(y/y_o)$; $10^{x/x_o} = 10^{\log_{10}(y/y_o)}=y/y_o \Rightarrow y = y_o10^{x/x_o}$
   \else
   \vspace{2em}
   \fi

# Introduction -- Base $e$ Logarithm

The base $10$ logarithm reduces numbers raised by a power of 10 to the power the number was raised to.

The base $e$ logarithm reduces numbers raised by a power of $e$ to the power the number was raised to. It is represented by $\log_{e}x$, or more commonly, $\ln(x)$.

"$\ln$" represents the "natural logarithm". The term "natural" is used because the exponential $e$ appears in many natural problems, for example, some populations grow in proportion to $e^{t/\tau}$, where the constant $\tau$ is a growth rate.

In mathematical notation, $\ln(e^x) = x$; for example $\ln(e^{-5}) = -5$ and $\ln(e^7) = 7$

Several identities follow as a result:

1. If you raise a base-$e$ logged number by $e$, you get back the number that was logged.

   $e^{\ln(x)} = x$

2. The sum of two logged numbers is the log of the product of the numbers:

   $\ln(y) + \ln(x) = \ln(yx)$;

3. The difference between two logged number is the log of the ratio of the numbers:
 
   $\ln(y) - \ln(x) = \ln(y/x)$

## Problems


1. What is $\ln(e^3)$?

   \ifsolutions
   **Answer**: $3$
   \else
   \vspace{2em}
   \fi

2. What is $\ln(1/e^3)$?

   \ifsolutions
   **Answer**: $-3$
   \else
   \vspace{2em}
   \fi

3. $\ln(e^{-4})+\ln(e^{3}) = \ln(x)$. Find $x$

   \ifsolutions
   **Answer**: $\ln(e^{-4})+\ln(e^{3})=\ln(e^{-4}\cdot e^{3})=\ln(e^{-1})=-1$
   \else
   \vspace{2em}
   \fi

4. $\ln(e^{-4})-\ln(e^{3}) = \ln(x)$. Find $x$.

   \ifsolutions
   **Answer**: $\ln(e^{-4})-\ln(e^{3})=\ln(e^{-4}/e^{3})=\ln(e^{-7})=-7$
   \else
   \vspace{2em}
   \fi

5. If $x = x_o\ln(y/y_o)$, solve for $y$ in terms of $x$.

   \ifsolutions
   **Answer**: $x/x_o = \ln(y/y_o)$; $e^{x/x_o} = e^{\ln(y/y_o)}=y/y_o \Rightarrow y = y_oe^{x/x_o}$
   \else
   \vspace{2em}
   \fi


