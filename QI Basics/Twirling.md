
# Twirling

퀀텀 채널에서 임의의 에러를 pauli error 로 바꿔주는 것.


## Pauli Twirling

twirling set is subset of pauli set

- Gottesman-Knill theorem. This
theorem states that any quantum circuit consisting only of
Clifford-group unitaries and measurement in the Pauli basis
can be simulated classically in polynomial time

each time we run the circuit, we conjugate the noise operator M with a different wirling gate w from the twirling set W.

pauli gate set

I, X, Z, Y

- I : identity
- X: bit flip
- Z : phase flip
- Y : bit+phase flip

어떠한 프로세스 $\Lambda$ 에 대해서, 파울리행렬의 제곱은 identity 고, 큐빗은 파울리 행렬의 베이시스 벡터로 표현될 수 있으니, 만약 파울리 베이시스로 표현되지 않는 에러가 없다면 $X^{-1}\Lambda X$ 를 지난 큐빗은 아무런 변화가 없어야 함.