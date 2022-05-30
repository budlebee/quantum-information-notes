# Time reversal operator (Motion reversal operator)

Time reversal is a misnomer; more appropriate term is motion reversal. Indeed, E. Wigner, who formulated time reversal, used "reversal of motion".

In classical view, time reversal means $x\rightarrow x,p\rightarrow -p.$

In quantum view, time reversal operator is complex conjugation operator. 

$$
\hat{T}\psi(x,t)=\psi^*(x,-t)
$$

Let's consider schrodinger equation

$$
i\hbar \frac{\partial\psi}{\partial t}=(-\frac{\hbar^2}{2m}\nabla^2 +V)\psi
$$



Suppose $\psi(x,t)=e^{-iEt/\hbar}\psi(x,0)$ is a solution. We can verify that $\psi(x,-t)$ is not a solution but $\psi^*(x,-t)$ is a solution.

In position space, momentum operator is represented by $-i\hbar \frac{\partial}{\partial x}$

So defining time inversion operator as a complex conjugate operator is to makes sense.

$$
\hat{T}\psi=\psi^*\newline
 \hat{T^\dagger}\hat{x}\hat{T}=\hat{x}\newline
 \hat{T^\dagger}\hat{p}\hat{T}=-\hat{p}
 $$

## Anti Unitrarity

The transformation $U_A\ket{a} = \ket{a'}$, $U_A\ket{b} = \ket{b'}$ is said to be antiunitary if 

$$
\braket{b'|a'} = \braket{b|a}^*=\braket{a|b} \newline
U_A(c_1\ket{a}+c_2\ket{b})=c^*_1U_A\ket{a}+c^*_2U_A\ket{b}
$$

the second line is a property of antilinear operator.

Antiunitary operator can be written as $U_A = UK$, where $K$ is complex conjugate operator.

For infinitesimal time evolution $\delta t$, 
$$
(1-\frac{iH\delta t}{\hbar})\hat{T}\ket{\psi} = \hat{T}(1-\frac{iH(-\delta t)}{\hbar})\ket{\psi}
$$
![time_reversal.png](./fig/time_reversal.png)

The above relation is to be true for any ket, we must have

$$
-iH\hat{T}\ket{\psi}=\hat{T}iH\ket{\psi}
$$

This is why time reversal is anti unitary.

$\bra{b}\hat{T}\ket{a}$ is always to be understood as $\bra{b}(\hat{T}\ket{a})$, never as $(\bra{b}\hat{T})\ket{a}$.

In fact, we do not even attempt to define $\bra{b}\hat{T}$. Dirac bra-ket notation was invented to handle linear operators, not antilinear operators. 

## reference

Modern quantum mechanics, Sakurai