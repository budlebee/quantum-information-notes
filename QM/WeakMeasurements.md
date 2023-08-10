

# Quantum theory of measurements

어떤 시스템 $\ket{\psi_i}$ 가 있고, 이 시스템을 측정하는 측정기를 $\ket{\phi(x)}$ 라고 하자. 우리는 측정기의 눈금 위치를 읽음으로써 어떤 물리량에 대한 정보를 알아낼 수 있다. 

시스템에서 우리가 측정하고자 하는 물리량을 $\hat{A}$라 하면, 해당 물리량을 측정함으로써 눈금이 얼마나 움직일지를 결정할 상호작용 해밀토니안은 다음과 같이 쓸 수 있다.

$$
\hat{H}_{int} = g\hat{A}\otimes \hat{p}
$$
여기서 $g$ 는 시스템과 측정기가 어느정도로 커플링 되었는지를 나타내는 값이다. 

측정을 통한 시스템의 time evolution 은 다음과 같이 쓸 수 있다 (편의상 $\hbar=1$ 으로 썼다.)

$$
e^{-i\int \hat{H}_{int} dt}\ket{\psi_i}\ket{\phi(x)} = (1-i\int \hat{H}_{int} dt+...)\ket{\psi_i}\ket{\phi(x)}
$$

이때 시스템과 측정기가 약하게 커플링 돼 있다면, 즉 $H_{int}$ 가 작다면, higher-order 를 날려버리는 식으로 approximation 이 가능하다.

$$
e^{-i\int \hat{H}_{int} dt}\ket{\psi}\ket{\phi(x)} \simeq (1-i\int \hat{H}_{int} dt)\ket{\psi_i}\ket{\phi(x)}\\
=(1-i\int g\hat{A}\otimes\hat{p} dt)\ket{\psi_i}\ket{\phi(x)}
$$

이 상황에서 시스템을 어떤 상태, $\bra{\psi_f}$ 로 프로젝션 시켜보자.

$$
\bra{\psi_f}(1-i\int g\hat{A}\otimes\hat{p} dt)\ket{\psi_i}\ket{\phi(x)}\\
=(\braket{\psi_f|\psi_i}- i\int g dt\bra{\psi_f}\hat{A}\ket{\psi_i}\hat{p})\ket{\phi(x)}
$$

여기서 weak value $A_w$ 를 정의하자.

$$
A_w := \frac{\bra{\psi_f}\hat{A}\ket{\psi_i}}{\braket{\psi_f|\psi_i}}
$$

weak value 의 정의를 활용해서 식을 다시 쓰면,

$$
\braket{\psi_f|\psi_i}- i\int g dt\bra{\psi_f}\hat{A}\ket{\psi_i}\hat{p}\ket{\phi(x)}\\
= \braket{\psi_f|\psi_i}(1-iA_w\int g dt \hat{p})\ket{\phi(x)}
$$

여기서 $g$ 를, 시스템과 측정기 사이의 impulse interaction 이라고 생각하면(일종의 델타펑션으로 생각하면), $\int gdt=1$ 로 쓸 수 있고, 위 식은 다음과 같이 쓸 수 있다. 


$$
\braket{\psi_f|\psi_i}(1-iA_w\int g dt \hat{p})\ket{\phi(x)}\\
\simeq \braket{\psi_f|\psi_i} e^{-iA_w \hat{p}}\ket{\phi(x)}=\braket{\psi_f|\psi_i}\ket{\phi(x-A_w)}
$$


$e^{-iA_w \hat{p}}$ 가 위치 translation operator 이므로, 우리 측정기의 눈금이 weak value $A_w$ 만큼 움직인걸 확인할 수 있다.

여기서 시스템의 초기상태와 최종상태의 오버랩 $\braket{\psi_f | \psi_i}$ 이 작으면 작을수록, weak value 의 정의에 따라 $A_w$ 의 값이 커진다. 오버랩을 작게 만들수록 우리 측정기의 눈금이 움직이는 정도를 증폭할 수 있는 것이다. 이런 테크닉을 weak value amplification 이라고 한다.

하지만 오버랩이 작으면 작을수록 wavefunction 앞에 붙는 amplitude $\braket{\psi_f | \psi_i}$ 의 값도 작아진다. 즉, 측정을 위해서는 입자를 많이 소모해야 된다는 trade-off 가 있다.

또한 이런 approximation 은 higher-order terms 를 무시했기 때문에 유효한 것이기에, 오버랩을 너무 작게 해서 $A_w$ 값이 너무 커지면 break down 이 일어난다. 

이런 weak value 를 이용한 메트롤로지는 비유적으로 표현하자면 통계적인 세척이라고 볼 수 있는데, 1/f 노이즈 같은 몇몇 노이즈에 대해서 이득을 얻을 수 있다고 한다.