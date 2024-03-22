
## Angular momentum of non-degenerate stationary state

Non-degenerate stationary state (observable 들이 time-independent 한 상태, energy eigenstate) 에서는 rotation angular momentum $\hat{L}=0$ 이다.

Stationary state 이니 $t\rightarrow -t$ 인 inversion 이 있어도 energy 가 변하지 않고, non-degenerate 이니 energy 가 변하지 않았다면 state 도 변하지 않았다는 것인데, $t\rightarrow -t$ 인 time inversion 에 대해서 $\hat{L} \rightarrow -\hat{L}$ 이므로 $\hat{L} = -\hat{L}$ 이니 $\hat{L}=0$ 이 된다.

수학적인 증명은 다음과 같다. non-degenerate stationary state 는 wave function 이 real function 이므로(stationary state 는 time reversal symmetry 가 있고, time reversal 연산자가 wave function 에 가해지면 complex conjugate 가 되는데, $\psi = \psi^*$ 이므로 real function 이다) L 의 expectation value 는

$$
\langle L\rangle = \int dr \psi^* \hat{L}\psi \\
= -i\hbar \int dr \psi^*(\hat{r}\times\nabla)\psi
$$

이때 적분 안쪽의 값은 전부 real 인데 밖에 i 가 곱해져 있으므로 $\langle L\rangle$ 는 pure imaginary 인데, expectation value 는 정의상 real 이어야 하므로 $\langle L\rangle=0$ 이다.

# angular momentum eigenstate basis

AM operator 에 대한 eigenstate 의 베이시스를 표현하는 법은 크게 두가지가 있음.

## option A

operator $J_1^2$, $J_2^2$,$J_{1z}$,$J_{2z}$ 와 $\ket{j_1,j_2,m_1,m_2}
$

$\ket{\uparrow\downarrow}$ 상태의 경우 $j_1 = 1/2$, $j_2 = 1/2$, $m_1 = 1/2$, $m_2 = -1/2$ 이므로

$$
\ket{\uparrow\downarrow} = \ket{j_1=1/2,j_2=1/2,m_1=1/2,m_2=-1/2}
$$


## example : $S_1 \cdot S_2\ket{\Psi^-}$ 계산하기


option B $\ket{j_1,j_2,j,m}$ 로 상태를 표현하면

$$
\ket{\Psi^-} = \frac{1}{\sqrt{2}}(\ket{\frac{1}{2},\frac{1}{2},0,0}-\ket{\frac{1}{2},\frac{1}{2},0,0})
$$

$$
\bold{S_1\cdot S_2} = \frac{1}{2}(\bold{S^2 - S_1^2 -S_2^2})
$$

$$
S^2\ket{\Psi^-} = 0
$$
$$
S_1^2\ket{\Psi^-} = s(s+1)\hbar^2\ket{\Psi^-} = \frac{3}{4}\hbar^2 
$$
$$
S_2^2\ket{\Psi^-} = s(s+1)\hbar^2\ket{\Psi^-} = \frac{3}{4}\hbar^2 
$$

$$
\bold{S_1\cdot S_2}\ket{\Psi^-} = \frac{1}{2}(0-\frac{3}{4}\hbar^2-\frac{3}{4}\hbar^2) = -\frac{3}{4}\hbar^2
$$

spin triplet state 들의 경우, s=1 이므로, $S^2\ket{j_1,j_2,s=1,m}=s(s+1)\hbar^2\ket{j_1,j_2,s=1,m} = 2\hbar^2\ket{j_1,j_2,s=1,m}$ 이므로 eigenvalue 는

$$
\frac{1}{2}(2\hbar^2-\frac{3}{4}\hbar^2-\frac{3}{4}\hbar^2) = \frac{1}{4}\hbar^2
$$

가 된다.


>note

$$
\bold{S_1\cdot S_2} = \bold{S_{1z}S_{2z}} +\frac{1}{2}(\bold{S_1^+ S_2^- +S_1^- S_2^+})
$$

where $S^+ = S_x +iS_y$, $S^- = S_x -iS_y$

## References

Landau Quantum Mechanics 3rd edition, Section 26.