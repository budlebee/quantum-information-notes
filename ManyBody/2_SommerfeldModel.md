Drude model : Boltzmann distribution

Sommerfeld model : Fermi-Dirac distribution

Fermi-Dirac distribution

$$
f(\varepsilon) = \frac{1}{e^{(\varepsilon-\mu)/k_B T}+1}
$$

where $\varepsilon$ is a system energy and $\mu$ is a chemical potential. 

chemical potential : 입자수가 보존되는 경우에만 화학 포텐셜이 있다. 온도에 대한 함수임 $\mu(T)$.

BEC 가 일어나려면 입자수가 보존돼야 함.

입자수가 고정돼 있지 않으면 BEC 가 안됨. 예를 들어 광자는 입자수가 보존 안되므로 BEC 가 안됨.

Density of States (DOS) $g(\varepsilon)$ : 해당 에너지의 degeneracy.

Sommerfeld expansion


절대영도 일때 분포 $f_0(\varepsilon)$

온도가 낮을수록 higher order 가 필요 없어진다.

절대영도일때의 화학 포텐셜 = Fermi energy $\varepsilon_F$.

화학케미컬은 온도의 함수이므로 페르미 에너지로 approximation.

DOS $g(\varepsilon)$ 의 기울기가 음수면 화학포텐셜이 올라가고 $g(\varepsilon)$ 의 기울기가 양수면 화학포텐셜이 내려간다.

중요: 

$$
u = u_0 + \frac{\pi^2}{6}(k_B T)^2 g(\varepsilon_F)
$$

$u_0$ : zero temp energy per volume. DOS $g(\varepsilon)$ 를 측정할때 위 formula 를 씀. 

specific heat 전자에 의한 것 T. 포논에 의한 것 T^3 in low T.

specific heat : 평형상태 property. conductivity 는 비평형 상태의 property 라 외부 영향을 받기 쉬움.

specific heat 을 실험적으로 측정하는 것 쉬운 일이 아님. 많은 노하우가 필요함. 이거 잘 측정하면 세계적인 그룹. 보통 신물질의 specific heat을 측정하는데 그런 신물질은 샘플 양이 적은 편임. 그런거 재는거 쉽지 않음.

sp heat 재는 그룹은 DFT 그룹이랑 초기부터 콜라보를 많이함. DOS 를 계산해 달라 

초전도 물질 $g_{measure} =(1+\lambda)g_{system}$. $\lambda$는 0.5 나 1.

보통 논문에선 specific heat 을 per volume 이 아니라 per mole 이나 per gram 으로 발표함. 왜냐면 volume 은 열팽창이 약간 있어서 유효숫자를 깎아먹음.

전자의 wave packet 은 1A 정도 크기. 그럼 mean free path 단위가 수십A 정도면 전자의 움직임을 particle 로 생각하기 힘들다. 

하지만 보통 mean free path 가 수백A 정도 크기면 particle 로 approximation 해도 괜찮다.