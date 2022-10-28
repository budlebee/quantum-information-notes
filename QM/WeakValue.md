# 1. Applications of Weak value

실험에서 weak value 의 주된 3가지 활용

1. evolution parameter 로 사용. large weak value 는 detector signal 을 증폭시키거나, 예민한 unknown small evolution parameter 를 추측하는데 사용될 수 있다. (beam deflection, frequency shift, phase shift)

2. complex quantity 를 직접 측정하기.

3. conditioned average of generalized observable eigenvalues 역할.  Hardy's paradox 나 three-box paradox 등 과 연결이 있다고 한다. 

# 2. What is a Weak value?

Let initial state is $\ket{i}$ and final state is $\ket{f}$. detection probability of $\ket{f}$ from $\ket{i}$ is $P=|\braket{f|i}|^2$.

If initial state is modified by some unitary operator $U(\epsilon)$ (parametrized by $\epsilon$), detection probability becomes $P_\epsilon=|\braket{f|U(\epsilon)|i}|^2$.

For some Hermitian operator $A$ (generator of unitary $U(\epsilon)$), we can write it as follows:

$$
U(\epsilon) = e^{-i\epsilon A} = 1-i\epsilon A + O(\epsilon^2)
$$

Thus,

$$
P_\epsilon = |\braket{f|U(\epsilon)|i}|^2 = |\bra{f}1-i\epsilon A+...\ket{i}|^2\newline
= (\braket{f|i}-i\epsilon\bra{f}A\ket{i}+...)\times (\braket{i|f}-i\epsilon\bra{i}A\ket{f}+...)\newline
= |\braket{f|i}|^2 +i\epsilon\braket{f|i}\bra{i}A\ket{f} - i\epsilon \bra{f}A\ket{i}\braket{i|f}+O(\epsilon^2)
$$

이때 $c=\alpha+i\beta$, $c^*-c = -2i\beta=-2i\Im{c}$ 이고, $(\bra{f}A\ket{i}\braket{i|f})^* = \braket{f|i}\bra{i}A\ket{f}$ 이므로

$$
P_\epsilon  = P +2\epsilon \Im(\bra{f}A\ket{i}\braket{i|f}) + O(\epsilon^2) 
$$

이고, 여기서 Weak value 를 $A^n_w = \frac{\bra{f}A\ket{i}}{\braket{f|i}}$ 로 정의한다면

$$
\frac{P_\epsilon}{P} = 1+2\epsilon \Im{A_w} + O(\epsilon^2)
$$

로 쓸 수 있다.

이때 parameter $\epsilon$ 의 크기가 충분히 작거나, first order weak value $A_w$ 의 값이 higher order 에 비해 충분히 크다면 higher order 들을 무시할 수 있다. 

대개의 경우 first order weak value 만 봐도 되는 상황을 만들어서 실험한다. 만약 처음 상태와 마지막 상태의 차이가 커서 $P=|\braket{f|i}|^2\rightarrow 0$ 라면 higher order Weak value 의 값이 커져서 무시할 수 없게 된다.

# 3. How to measure a Weak value?

## ref 

Understanding quantum weak values: Basics and applications, review of modern physics, volume 86, Jan-Mar 2014


