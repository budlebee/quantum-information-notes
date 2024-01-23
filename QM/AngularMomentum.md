
## Angular momentum of non-degenerate stationary state

Non-degenerate stationary state (observable 들이 time-independent 한 상태, energy eigenstate) 에서는 rotation angular momentum $\hat{L}=0$ 이다.

Stationary state 이니 $t\rightarrow -t$ 인 inversion 이 있어도 energy 가 변하지 않고, non-degenerate 이니 energy 가 변하지 않았다면 state 도 변하지 않았다는 것인데, $t\rightarrow -t$ 인 time inversion 에 대해서 $\hat{L} \rightarrow -\hat{L}$ 이므로 $\hat{L} = -\hat{L}$ 이니 $\hat{L}=0$ 이 된다.

수학적인 증명은 다음과 같다. non-degenerate stationary state 는 wave function 이 real function 이므로(stationary state 는 time reversal symmetry 가 있고, time reversal 연산자가 wave function 에 가해지면 complex conjugate 가 되는데, $\psi = \psi^*$ 이므로 real function 이다) L 의 expectation value 는

$$
\langle L\rangle = \int dr \psi^* \hat{L}\psi \\
= -i\hbar \int dr \psi^*(\hat{r}\times\nabla)\psi
$$

이때 적분 안쪽의 값은 전부 real 인데 밖에 i 가 곱해져 있으므로 $\langle L\rangle$ 는 pure imaginary 인데, expectation value 는 정의상 real 이어야 하므로 $\langle L\rangle=0$ 이다.

## References

Landau Quantum Mechanics 3rd edition, Section 26.