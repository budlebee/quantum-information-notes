# PT-symmetric Hamiltonian

If the Hamiltonian H commute with PT operator($[H,PT]=0$), then Hamiltonian have real energy eigenvalue spectra, even it is not Hermitian. 

## Parity operator P

P is parity inversion operator. In real space, parity inversion makes $(x,y,z) \rightarrow (-x,-y,-z)$. Quantum mechanically, 
$$
\hat{P}\psi(x)=\psi(-x)\\
 \hat{P}\hat{x}\hat{P^\dagger}=-\hat{x}
 $$
In 2x2 spin space, parity inversion is given by spin inversion operator, pauli X gate.
$$
\hat{P} = \begin{bmatrix}
0&1\\
1&0
\end{bmatrix}=\sigma_{x}
$$

## Time inversion operator T

Time reversal is a misnomer; more appropriate term is motion reversal. Indeed, E. Wigner, who formulated time reversal, used "reversal of motion".

In classical view, time inversion means $x\rightarrow x,p\rightarrow -p.$

In quantum view, time inversion operator has complex conjugation operation. 

$$
\hat{T}\psi(x)=\psi^*(x)
$$

Time reversal operator is system dependent; it is defined differently in spinless system and spin half system.

From classical analogy, operator transforms by time reversal are given by

$$
\hat{T}\psi=\psi^*\\
 \hat{T}\hat{x}\hat{T^{-1}}=\hat{x}\\
 \hat{T}\hat{p}\hat{T^{-1}}=-\hat{p}\\
  \hat{T}\hat{\sigma}\hat{T^{-1}}=-\hat{\sigma}
 $$

 where $\sigma$ is a spin angular momentum.

Time inversion operator is anti-unitary operator. Anti unitray operator $U^{\dagger}_{A} U_A=I$. But $\braket{U_A\phi |U_A\psi}=\braket{\psi|\phi}$, not $\braket{\phi|\psi}$. And $U_A \lambda \ket{\psi}=\lambda^* U_A\ket{\psi}$

By properties of antilinearity, we can say $THT^{-1}=H^{\dagger}$.

More details and motivations about time reversal are in my "Time Reversal" note.

## Simple proof that PT symmetric Hamiltonian has real real energy eigenvalue spectra

Let $\psi$ is a common eigenstate of $PT$ and $H$.

PT symmetry $[H,PT]=0$ means $HPT\ket{\psi}=PTH\ket{\psi}$.

 Let eigenvalue of PT operator is a $\lambda$.

 Left hand side is $\rightarrow H\lambda\ket{\psi}=E\lambda\ket{\psi}$.

 Right hand side is $PTE\ket{\psi}=E^* PT\ket{\psi}=E^*\lambda\ket{\psi}$, because $T$ operator is antilinear operator.

 By PT symmetry condition, left hand side = right hand isde. It meanse $E^* = E$. PT symmetric Hamiltonians have real energy eigenvalue spectra.

 Detailed proof are in reference *PT-symmetry in optics*.


## example

if and only-if condition of PT symmetric Hamiltonian is as follows:

$$
PTH(PT)^{-1} = PTHT^{-1}P^{-1}=PH^{\dagger}P^{-1}=H
$$

Because $P^{-1}=P$, we can say $PH^{\dagger}P^{-1}=H$ is the if and only-if condition of PT symmetric Hamiltonian.

Some 2x2 Hamiltonian is PT symmetric. For example,

$$
H=\begin{bmatrix}
re^{i\theta} && s\\
s && re^{-i\theta}
\end{bmatrix}
$$

$r,\theta,s$ are real quantity. Above is a PT symmetric Hamiltonian, $[H,PT]=0$.


## references

- Real Spectra in Non-Hermitian Hamiltonians Having PT Symmetry(1998), Carl M. Bender, Stefan Boettcher, prl 80, 24
- PT-symmetry in optics(2014), A.A. Zyablovsky et al.
- Modern quantum mechanics 3rd edition Chapter 4, J.J. Sakurai
- PT symmetry in quantum physics: from a mathematical curiosity to optical experiments(2016), Carl M. Bender


