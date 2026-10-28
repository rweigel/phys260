
\section{Calculating the magnetic field of a steady current}

The Biot-Savart law gives the magnetic field due to a steady current. 

\begin{center}
\includegraphics[]{Magnetic Fields Tutorial #3/figures/BiotSavart.png}
\end{center}

The magnetic field created by a small segment $d\mathbf{l}$ of a wire carrying a current $I$ is

$$d{\bf B} = \frac{\mu_0}{4\pi}\frac{I d{\bf l} \times \hat{\bf r}}{r^2}$$

where $\hat{\bf r}$ is a unit vector in the direction of the vector distance ${\bf r}$ from the source $d\mathbf{l}$ to the field point.

The Biot-Savart law can be used to find the total magnetic field ${\bf B}$ at any point in space due to all current elements (e.g., in a circuit) by summing the magnetic field created by each infinitesimal current element:

$${\bf B} = \frac{\mu_0}{4\pi}\int \frac{I d{\bf l} \times \hat{\bf r}}{r^2}$$

If the vector direction of the cross product does not change, this formula simplifies. Writing the magnitude of the cross product in the integral, $|d{\bf l} \times \hat{\bf r}|$, as $dl \sin \theta$, where $\theta$ is the angle between $d\mathbf{l}$ and $\hat{\bf r}$, the the magnetic field in the direction of the cross product can be written as

$$B = \frac{\mu_0}{4\pi}\int \frac{I\sin\theta dl}{r^2}$$

and the direction of the magnetic field must be determined using the right-hand rule.

\clearpage
\begin{tcolorbox}[enhanced,breakable,parbox=false,colback=white!0!white,colframe=blue!100!blue,title=Example 3.1]

The wire in the following figure is infinitely long and carries a current I. Calculate the magnitude and direction of the magnetic field produced at P.

\begin{center}
    \includegraphics[]{Magnetic Fields Tutorial #3/figures/BiotSavartExample1.png}
\end{center}

In this problem, apply the Biot-Savart law for both the horizontal and vertical segments of the wire for calculating the magnetic field at $P$. 

{\bf Step 1:} The magnetic field due to the horizontal wire is:

$$B_{horizontal} = \frac{\mu_0 I}{4\pi}\int \frac{dl\sin\theta}{r^2}$$

Because the direction of the vector $\mathbf{r}$ drawn from $d\mathbf{l}$ to point $P$ is in the same direction as $d\mathbf{l}$, $\theta = 0$ and so $\sin\theta = 0$, giving

$$B_{horizontal} = 0$$

{\bf Step 2:} From the right-hand rule, the magnetic field due to each small current element on the vertical wire will be parallel to the $z$ axis. As a result, we can used the simplified Biot-Savart formula:

$$B_z^{vertical} = \frac{\mu_0 I}{4\pi}\int \frac{dl\sin\theta}{r^2}$$

\begin{center}
    \includegraphics[scale = 0.5]{Magnetic Fields Tutorial #3/figures/BiotSavartExample2.png}
\end{center}

From the diagram, $dl = dy$, $r = \sqrt{y^2 + a^2}$, and

$$\sin \theta = \frac{a}{\sqrt{y^2 + a^2}}.$$

Therefore, 

$$B_z^{vertical} = \frac{\mu_0 I}{4\pi}\int_{y=0}^{-\infty} \frac{ady}{(a^2 + y^2)^{3/2}}$$

From a table of integrals,

$$\int \frac{dy}{(a^2 + y^2)^{3/2}} =  \frac{y}{a^2\sqrt{a^2 + y^2}} + C$$

$$B_z^{vertical} = \frac{\mu_0 I}{4\pi}\int_{y=0}^{-\infty} \frac{ady}{(a^2 + y^2)^{3/2}} = \frac{\mu_0 I}{4\pi}\frac{y}{a\sqrt{a^2 + y^2}}\Big|_0^{-\infty} = -\frac{\mu_0 I}{4\pi a}$$

{\bf Step 3: } Combining both ${\bf B}_{horizontal}$ and ${\bf B}_z^{vertical}$, the magnitude of the magnetic field {\bf B} is ${\mu_0 I}/{4\pi a}$, and the direction of {\bf B} at $P$ is perpendicular to the plane of the page and points out of the page. (The negative sign in the answer means that $\mathbf{B}^{vertical}$ has a negative $z$ component. By the right-hand rule, the $+z$ direction must be into the page for the coordinate axes given on the diagram.)

\begin{center}
\begin{subfigure}{}
\includegraphics[scale=1.2]{Magnetic Fields Tutorial #3/figures/RightHandRule2.png} 
\end{subfigure}
\begin{subfigure}{
\includegraphics[scale=1.2]{Magnetic Fields Tutorial #3/figures/RightHandRule3.png}
\end{subfigure}
\end{center}

\end{tcolorbox}
