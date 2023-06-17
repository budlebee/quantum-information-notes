Amplitude damping : excited state atom emits photon by interacting vacuum field (spontaneous emission).

ground state atom : $\ket{0}_A$

excited state atom : $\ket{1}_A$

vacuum field : $\ket{0}_E$

emitted photon : $\ket{1}_E$

If there are no external fields (environment is initially $\ket{0}_E$), spontaneous emission is written as follows

$$
U\ket{0}_A\ket{0}_E = \ket{0}_A\ket{0}_E
$$

$$
U\ket{1}_A\ket{0}_E = \sqrt{p}\ket{0}_A\ket{1}_E +\sqrt{1-p}\ket{1}_A\ket{0}_E
$$

$p=\Gamma t/n$ is spontaneous emission probability. $\Gamma$ is atom scattering rate. $t/n=\Delta t$ is collision time interval.

our initial system is 

$$
\rho \otimes \ket{0}\bra{0}
$$

Deriving Kraus operator $A_0$ and $A_1$ and superoperator $S[\rho]=A_0 \rho A_0^\dagger +A_1 \rho A_1^\dagger$

$$
A_0 = \bra{0}_E U \ket{0}_E = Tr_E[U(I\otimes \ket{0}\bra{0})]\\
= Tr_E[U(\ket{00}\bra{00} +\ket{10}\bra{10} )]\\
= Tr_E[\ket{00}\bra{00} + \sqrt{p}\ket{01}\bra{10}+\sqrt{1-p}\ket{10}\bra{10}]=\begin{pmatrix}1&0\\0&\sqrt{1-p}\end{pmatrix}
$$

$$
A_1 = \bra{1}_E U \ket{0}_E = Tr_E[U(I\otimes \ket{0}\bra{1})]\\
= Tr_E[U(\ket{00}\bra{01} +\ket{10}\bra{11} )]\\
= Tr_E[\ket{00}\bra{01} + \sqrt{p}\ket{01}\bra{11}+\sqrt{1-p}\ket{10}\bra{11}]=\begin{pmatrix}0&\sqrt{p}\\0&0\end{pmatrix}
$$

Thus, 

$$
S[\rho] = \begin{pmatrix}
\rho_{00}+p\rho_{11}&\sqrt{1-p}\rho_{01}\\\sqrt{1-p}\rho_{10}&(1-p)\rho_{11}\end{pmatrix}
$$

acting superoperator n times on $\rho$ :

$$
S^{\otimes n}[\rho] =
\begin{pmatrix}
\rho_{00}^{(n)} & \rho_{01}^{(n)}\\ \rho_{10}^{(n)}&\rho_{11}^{(n)}\end{pmatrix}
= 
\begin{pmatrix}
\rho_{00}^{(n-1)}+p\rho_{11}^{(n-1)}&\sqrt{1-p}^n\rho_{01}\\\sqrt{1-p}^n\rho_{10}&(1-p)^n\rho_{11}\end{pmatrix}
$$

수열 점화식을 풀면, $n \rightarrow \infty$ 일때 $(1-p)^n = (1-\Gamma t/n)^n \rightarrow e^{-\Gamma t}$ 이므로

$$
\rho(t) = \begin{pmatrix}
\rho_{00}+(1-e^{-\Gamma t})\rho_{11}& e^{-\Gamma t/2}\rho_{01}\\ e^{-\Gamma t/2}\rho_{10}&e^{-\Gamma t}\rho_{11}\end{pmatrix}
$$

