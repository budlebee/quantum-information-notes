# total angular momentum

$$
\ket{l}\otimes\ket{s}
$$
$$
\bold{J} = \bold{L} \otimes \bold{1} + \bold{1}\otimes \bold{S} \equiv \bold{L}+\bold{S}
$$

rotation operator is

$$
D(R) = D^{orbit}(R)\otimes D^{spin}(R) = e^{-i\bold{L}\cdot\hat{\bold{n}}\phi/\hbar} \otimes  e^{-i\bold{S}\cdot\hat{\bold{n}}\phi/\hbar}
$$

# spin addition

$$
\bold{S =S_1\otimes 1 + 1\otimes S_2 =  S_1 +S_2}
$$

local operators for other party commute each other.
$$
[S_1,S_2] = 0
$$


total spin operator does not commute
$$
[S_x,S_y] = i\hbar S_z
$$

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