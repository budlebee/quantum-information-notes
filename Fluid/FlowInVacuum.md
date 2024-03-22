## Knudsen number

기체의 mean free path $\lambda$를 기체관의 diameter $D$와 비교 했을때, $\lambda$ 가 훨씬 작다면 유체의 흐름은 관과의 충돌보다 유체끼리의 충돌이 훨씬 많을 것이고(viscous flow), $\lambda$ 가 훨씬 크다면 관과의 충돌이 훨씬 많을 것이다(molecular flow). 이때, Knudsen number $K_n$은 다음과 같이 정의된다.

$$
K_n=\frac{\lambda}{D}
$$

* $K_n < 0.01 \rightarrow$ viscous flow

* $0.01 < K_n < 1\rightarrow$ transition flow

* $1 < K_n\rightarrow$ molecular flow


## 유량과 컨덕턴스

진공에서 기체량은 압력x용적, 유량 $Q$는 압력x용적/시간으로 나타낸다. 유량의 단위는 $Pa\cdot m^3/s$, $Torr\cdot I/s$ 등이 있다.

진공배관에서 컨덕턴스 C는 유량과 압력차의 비례관계를 나타내는 상수이다.

$$
Q = C(p_i - p_o)
$$

$p_i$ is the inlet pressure and $p_o$ is the outlet pressure.


## Mean free path

$$
\lambda = \frac{1}{\sqrt{2}n\sigma}
$$

여기서 n은 분자의 밀도, $\sigma$는 collision cross section 으로, 다른 원자끼리라면 $\pi (a_1+a_2)^2$ 인데, 같은 원자라면 반지름 $a_1=a_2=a$ 이므로 보통 원자의 diameter $d$ 를 이용해 표현해서 $\pi d^2$ 로 나타낸다.

## Example

Na의 경우 520K 에서 vapor pressure 0.23Pa, 밀도 $3.3\cdot10^{19}/m^3$ 

Li의 경우 620K 에서 vapor pressure 0.0013Pa, 밀도 $1.5\cdot10^{17}/m^3$

$PV=Nk_B T$ 이므로, 밀도는 $n=N/V$ 이므로 $n=\frac{P}{k_B T}$ 이다.

Na 의 kinetic collision diameter 를 찾지 못해서 일단 $d=0.5nm$ 로 상정했다 (copilot 은 Na 는 0.25nm, Li의 경우 0.3nm 라고 알려주지만 출처는 모르겠다). 

이 경우 Na 의 mean free path 는 $27.3mm$ 이고, 관의 직경이 3mm 인 경우 $K_n$은 9.1 이므로 molecular flow 이다. 

긴 실린더 관에서 molecular flow 의 경우 컨덕턴스는 반지름 $a$와 관의 길이 $L$ 에 대해 $a^3/L$ 에 비례하게 된다.

기존 a=1mm 에서 a=1.5mm 로 늘리면 $1.5^3=3.375$ 이므로 관의 길이를 3배 정도 늘려도 같은 컨덕턴스가 나온다.