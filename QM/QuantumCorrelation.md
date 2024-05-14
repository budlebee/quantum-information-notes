\section{Entanglement: Quantum correlation}

By definition, a quantum system is said to be entangled if its quantum state cannot be separable into a product of individual systems. For two qubits entangled state,
![](./fig/ab_classic.pdf)
\begin{linenomath*}
	\begin{align}
		|\psi\rangle_{12} \neq |\psi\rangle_1 \otimes |\psi\rangle_2   
	\end{align}
\end{linenomath*}

These inseparable entangled states give higher correlation than classical physics. We will derive classical correlation and quantum correlation that have analogies to each other. Following analysis is mainly based on Ref. \cite{peresBook}. \par
Let us consider classical correlation: a classical bomb, initially at rest, then explodes into two pieces, carrying opposite angular momentum $\vec{J}_1$ and $\vec{J}_2 = -\vec{J}_1$. Two separated observers measure the sign of angular momentum along arbitrary unit vector $\hat{\alpha}= \alpha_1 \hat{x}+\alpha_2 \hat{y}+\alpha_3 \hat{z}$ and $\hat{\beta}= \beta_1 \hat{x}+\beta_2 \hat{y}+\beta_3 \hat{z}$.

\begin{linenomath*}
	\begin{align}
		&a= sign(\hat{\alpha}\cdot \vec{J}_1) = \pm 1\\ \nonumber
		&b= sign(\hat{\beta}\cdot \vec{J}_2) = \pm 1
	\end{align}
\end{linenomath*}

This measurement is repeated $N$ times. Let $a_i$ and $b_i$ be the $i$th measurement results. If the angular momentum directions are random, the expectation values of repeated measurement are

\begin{linenomath*}
	\begin{align}
		&\langle a\rangle = \frac{1}{N}\sum_i a_i\\ \nonumber
		&\langle b\rangle = \frac{1}{N}\sum_i b_i,
	\end{align}
\end{linenomath*}

Two values become 0 when $N \rightarrow \infty$. 

If two observers compare their results, they can find a correlation of $a$ and $b$.

\begin{linenomath*}
	\begin{align}
		&\langle ab\rangle = \frac{1}{N}\sum_i a_i b_i
	\end{align}
\end{linenomath*}

This correlation depends on the angle between $\hat{\alpha}$ and $\hat{\beta}$. For example, if $\hat{\alpha}=\hat{\beta}$, $a$ and $b$ always are opposite values, so $\langle ab \rangle =-1$.

For arbitrary $\hat{\alpha}$ and $\hat{\beta}$, the correlation $\langle ab \rangle$ can be calculated as follows: An unit sphere, separated by the equatorial planes perpendicular to $\hat{\alpha}$ and $\hat{\beta}$. If $\vec{J}_1$ points upper hemisphere of $\hat{\alpha}$ plane, $\vec{J}_2$ places lower hemisphere. This case, $\langle a \rangle =1$ and $\langle b \rangle$ is 1 for $0$ to $\theta$ and -1 for $\theta$ to $\pi$. Thus, we can say that unit sphere is separated into four sections with alternating signs of $ab$ by two equatorial planes. 

If $\vec{J}_1$ is uniformly distributed in $[0,\pi]$, the classical correlation is


\begin{linenomath*}
	\begin{align}
		\langle ab\rangle = \frac{\theta}{\pi}\times 1 + \left(\frac{\pi-\theta}{\pi}\right)\times(-1) = \frac{2\theta}{\pi} - 1
		\label{eq_correlation}
	\end{align}
\end{linenomath*}

\begin{figure}[h]
	\centering
	\includegraphics[width=0.7\textwidth]{./picture/ch1/ab_classic.pdf}
	\caption{Geometric interpretation for Eq. (\ref{eq_correlation}). In the shaded area, classical correlation $\langle ab\rangle=1$ and $\langle ab\rangle=-1$ in the un-shaded.}
	\label{fig_classical_correlation}
\end{figure}

Now let us consider quantum correlation. Consider a spin singlet system, 

\begin{linenomath*}
	\begin{align}
		|\psi\rangle_{12} =\frac{|\uparrow\rangle_1 |\downarrow\rangle_2 -|\downarrow\rangle_1 |\uparrow\rangle_2 }{\sqrt{2}}   
	\end{align}
\end{linenomath*}

$|\uparrow\rangle$ and $|\downarrow\rangle$ represent the spin up and down in any measurement direction, respectively. Total spin of the system is 0 and the spin of each particle is opposite to the each other. Mathematically, this quantum state cannot be written in the separable form, so it is entangled state.\par
Now, the two particles are distributed to Alice and Bob, spatially. Alice's measurement of the spin along the direction to normalized vector $\hat{\alpha}$ is given by $\hat{\alpha}\cdot\vec{\sigma}^{(1)}$, where $\vec{\sigma}^{(1)} = \sigma_x \hat{x}+\sigma_y \hat{y}+\sigma_z \hat{z}$. The Pauli matrices are

\begin{linenomath*}
	\begin{align}
		\sigma_x =\begin{pmatrix}
		0 & 1\\
		1&0
		\end{pmatrix},
		\sigma_y =\begin{pmatrix}
			0 & -i\\
			i&0
		\end{pmatrix},
		\sigma_z =\begin{pmatrix}
			1 & 0\\
			0&-1
		\end{pmatrix}
	\end{align}
\end{linenomath*}

The average value of Alice's spin measurement $\langle a \rangle$ is as follows:

\begin{linenomath*}
	\begin{align}
		\langle a \rangle = \langle \psi| \hat{\alpha}\cdot\vec{\sigma}^{(1)} | \psi\rangle = 0
	\end{align}
\end{linenomath*}

Bob also obtains $\langle b \rangle = 0$. This results are same with classical expectation values when $N\rightarrow \infty$.\par
For the correlation $\langle ab\rangle$ of quantum state,

\begin{linenomath*}
	\begin{align}
		\langle ab \rangle = \langle \psi| (\hat{\alpha}\cdot\vec{\sigma}^{(1)}) (\hat{\beta}\cdot\vec{\sigma}^{(2)}) | \psi\rangle 
	\label{eq_ab}
	\end{align}
\end{linenomath*}

Following mathematical tricks make calculation more straight forward.

\begin{linenomath*}
	\begin{align}
		\hat{\beta}\cdot \vec{\sigma}^{(2)}|\psi\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix}
		\beta_1 - i\beta_2 \\
		-\beta_3\\
		-\beta_3\\
		-\beta_1 - i\beta_2 
		\end{pmatrix} = -\hat{\beta}\cdot \vec{\sigma}^{(1)}|\psi\rangle
		\end{align}
\end{linenomath*}

\begin{linenomath*}
	\begin{align}
		(\hat{\alpha}\cdot\vec{\sigma}^{(1)}) (\hat{\beta}\cdot\vec{\sigma}^{(1)})
		=\hat{\alpha}\cdot\hat{\beta} +i (\hat{\alpha}\times\hat{\beta})\cdot\vec{\sigma}^{(1)}  
	\end{align}
\end{linenomath*}

Then Eq. (\ref{eq_ab}) is calculated to

\begin{linenomath*}
	\begin{align}
		&\langle \psi| (\hat{\alpha}\cdot\vec{\sigma}^{(1)}) (\hat{\beta}\cdot\vec{\sigma}^{(2)}) |\psi\rangle
		= -\langle \psi| (\hat{\alpha}\cdot\hat{\beta} +i (\hat{\alpha}\times\hat{\beta})\cdot\vec{\sigma}^{(1)} )|\psi\rangle \\ \nonumber
		&= -\frac{1}{2}\begin{pmatrix} 0 & 1&-1&0 \end{pmatrix} \cdot
		\begin{pmatrix} 
		-i(\alpha_2 \beta_3 -\alpha_3\beta_2) -(\alpha_3\beta_1 -\alpha_1\beta_3) \\
		\hat{\alpha}\cdot \hat{\beta} +i(\alpha_1\beta_2-\alpha_2\beta_1) \\
		-\hat{\alpha}\cdot \hat{\beta} +i(\alpha_1\beta_2-\alpha_2\beta_1) \\
		i(\alpha_2\beta_3 - \alpha_3\beta_2)-(\alpha_3 \beta_1 -\alpha_1\beta_3) \end{pmatrix}= - \hat{\alpha}\cdot \hat{\beta} = -\cos{\theta}
	\end{align}
\end{linenomath*}

where the $\theta$ is angle between $\hat{\alpha}$ and $\hat{\beta}$.

Figure \ref{fig_correlation} shows the classical correlation and the quantum correlation. Entangled state gives higher correlation than classical physics. 

\begin{figure}[h]
	\centering
	\includegraphics[width=0.8\textwidth]{./picture/ch1/correlation.pdf}
	\caption{Quantum and classical correlation.}
	\label{fig_correlation}
\end{figure}
