amplitude damping 처럼 system 에 loss 가 있는 상황 -> 시스템 a와 환경 b 가 커플된 master equation 으로 기술. 상호작용 해밀토니안은 $H_I$.

환경을 trace out 하고 시스템에 대한 reduced density matrix 를 구하면 됨.

싱글모드파이버에서 빛이 밖으로 빠져나가는 것을 모델링하면 

$$
H_I = \chi (a^{\dagger}b+b^{\dagger}a)
$$
이때 a와 b는 시스템과 환경의 annihilation 연산자.

환경의 온도 kT는 시스템의 에너지 스케일 $\hbar w$ 에 비해 낮아서 $<b^{\dagger}b>=0$이고 시스템에서 환경으로만 포톤이 빠져나간다고 가정.

실제 실험상황에서는 input 과 output 의 값을 측정할 것이므로, 시스템의 연속적인 변화보다는 $t$와 $t+\triangle t$ 의 값이 관심사. 

그렇다면 시스템의 최종상태 $\rho'$는 다음과 같이 kraus 연산자로 표현할 수 있다.

$$
\rho' = \sum_{k}L_k \rho L_{k}^{\dagger}
$$

이때 $L_k$의 matrix element 는 다음과 같다.

$$
L_{k} = \bra{k}_b e^{iH_I \triangle t}\ket{0}_b
$$

operator algebra 로 계산하면, 

$$
L_k = \sum_{n} \sqrt{\begin{pmatrix}n\\k \end{pmatrix}}\sqrt{T^k R^{n-k}}\ket{n-k}\bra{n}
$$

memory 에 저장되는 상태를 보는 것이므로, k 가 빠져나가는 것은 $T^k$

annihilation 연산자와 n 에 대해 표현하다면,

$$
L_n = \bigotimes_{i}^{M} \sqrt{\frac{T^k R^{n_i -k_i}}{n_i!}}b^{n_i}
$$
