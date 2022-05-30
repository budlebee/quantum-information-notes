# PT-symmetry Hamiltonian ? 

Hamiltonian H 가 PT 와 commute 한다면 [H,PT] = 0 이라면, H 는 real eigenvalue spectra 를 가진다. 

## Parity operator P

space inversion operator. $\hat{P}\psi(x)=\psi(-x).\newline
 \hat{P^\dagger}\hat{x}\hat{P}=-\hat{x}$

## Time inversion operator T

In classical view, time inversion means $x\rightarrow x,p\rightarrow -p.$

In quantum view, time inversion operator is complex conjugation operator. 

$$
\hat{T}\psi(x)=\psi^*(x)
$$

It does not change probability distribution in position space.

In position space, momentum operator is represented by $-i\hbar \frac{\partial}{\partial x}$

So defining time inversion operator as a complex conjugate operator is to makes sense.

$$
\hat{T}\psi=\psi^*\newline
 \hat{T^\dagger}\hat{x}\hat{T}=\hat{x}\newline
 \hat{T^\dagger}\hat{p}\hat{T}=-\hat{p}
 $$

time inversion operator is anti-unitary operator. Anti unitray operator $U^{\dagger}_{A} U_A=I$. But $\braket{U_A\phi |U_A\psi}=\braket{\psi|\phi}$, not $\braket{\phi|\psi}$. And $U_A \lambda \ket{\psi}=\lambda^* U_A\ket{\psi}$

## How PT symmetric hamiltonian has real eigenvalue spectra? (tba)

Let $\psi$ is a common eigenstate of $PT$ and $H$.


## example

$$
H=\begin{bmatrix}
re^{i\theta} && s\\
s && re^{-i\theta}
\end{bmatrix}
$$
$r,\theta,s$ are real. Above is a PT symmetric, $[H,PT]=0$.

$$
PTH = HPT \rightarrow PTHT^{-1}=HP\rightarrow PTHT^{\dagger}=HP = PH^*
$$

In 2-dimension, P operator is pauli x operator. 