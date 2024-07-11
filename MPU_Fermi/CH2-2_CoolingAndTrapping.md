
* 방향 notation: 중력방향 또는 radial 방향이 x 방향이고, ODT 진행방향(중력과 수평한 방향)이 z 임.

* laser cooling & magnetic trapping: boson 이랑 똑같음.

* 동조냉각으로 $T_F$~$T_c$ 사이로 내리고, 리튬만 남았을때 ODT 증발냉각으로 $T_c$ 아래로 내린다.

* 넘버가 줄어들면 $T_F$ 도 줄어듬. 다이나믹스에 중요한 것은 $T/T_F$.

## Sympathetic cooling

두 종류의 원자 구름이 겹쳐있어야 함. 하지만 원자는 질량이 달라서 중력에 따른 sag 이 다름 (특히 Rb-Li 처럼 질량차이가 클수록 심함).

중력과 하모닉 트랩의 복원력의 관계 $mg = k\triangle x = m\omega^2 \triangle x$ 에 따른 수직방향 sag는

$$
\triangle x = \frac{g}{\omega^2} = \frac{mg}{k}
$$

하모닉 트랩의 스프링 상수는 
$$
k=m\omega^2 \simeq  
\begin{cases} 
 \mu_B B^{\prime\prime} &\text{for magnetic trap}\\
\alpha I^{\prime\prime}& \text{for optical trap}
\end{cases}
$$ 

$\mu_B$: 보어마그네톤, $B^{\prime\prime}$: 마그네틱 필드의 curvature, $\alpha$: 원자의 polarizability, $I^{\prime\prime}$: 레이저 인텐시티의 curvature. 알칼리 원자들의 polarizability 값은 유사하므로 스프링 상수 $k$ 는 원자에 무관하다고 볼 수 있다.
 
thermal cloud 의 사이즈를 $k r^2 \simeq k_B T$ 로 추정하면

$$
r_{\text{th}} \simeq \sqrt{k_B T/k}
$$

즉, 구름의 사이즈는 원자와 무관하게 trap 에 의해 결정되지만, sag 는 질량의 영향을 받는다. 두 원자 구름이 겹치기 위해서는

$$
\triangle x_1-\triangle x_2 = \frac{g(m_1-m_2)}{k}\simeq \sqrt{\frac{k_B T}{k}}
$$

두 원자 구름을 많이 겹치게 하고 싶다면 trap frequency 를 올려서 $k$ 값을 키우면 되지만, 그러면 three-body loss 가 심해짐.

* Fermion 이 Boson 보다 숫자가 많으면 냉각효율 떨어짐 (why?).

* Role of Fermi statistics: DFG 의 출현이 증발냉각의 kinetics 를 바꾸지만, Fermi temperature 아래로 내려가는 것을 막지는 않다. Ref: Evaporative cooling of a two-component degenerate Fermi gas, pra 61 053610. 레퍼런스 논문을 읽어본 바에 따르면 two-component Fermi 가스에서, dilute 인 경우 각각의 충돌 사이의 간격이 크기에 Markov 근사가 유효하고, thermalization rate 에 대한 Quantum Boltzman equation 을 세우면 최적의 evaporation 을 위한 parameter 를 계산해 나갈 수 있다고 한다. 

* DFG 의 경우 Fermi sea 에서의 hole excitation 때문에 background gas collision 같은 로스에 더 취약하다고 한다(why? ref: Degenerate Fermion Gas Heating by Hole Creation)

* BEC 의 heat capacity 는 0에 가깝지만, 아주 낮은 온도라서 일반적인 Bose 가스보다 더 Fermion 샘플을 냉각할 수 있다.

* Intraspecies scattering length: attractive 하거나 repulsive 하거나. Bose gas 의 밀도가 너무 높다면 attractive 상호작용이 많은 Fermion 들을 한데 뭉치게 해서 heating 과 loss 로 이어질 수 있다 (ref: Collapse of a degenerate Fermi gas, Science, 297 2240). (Q: 동조냉각할때 리튬보다 소듐 슬로워 등의 얼라인을 최적화 하는게 효과가 좋다는데, 냉각의 최적화된 Bose gas 의 밀도 스윗스팟을 찾아야 돼서 그런가?)

* RF 펄스와 decoherence 를 이용해 two-components mixture 를 만들면 maximum occupation 이 1/2 이 되고 effective $T/T_F$ 가 0.6이 되기 때문에, 그 아래로 냉각하는 것은 별 이득이 없다 (section 2.3.5 참고).

## Optical trap

AC Stark shift 를 이용한 trapping: 스핀 상태에 상관없이 붙잡을 수 있음.

High power laser 와 enhancement cavity 를 다룰 수 있다면 Magnetic trap 없이 all-optical trap 도 가능. $^6\text{Li}$의 경우 마그네틱 트랩을 안쓴다면 다른 원자를 쓸 필요가 없다.

red detune 된 가우시안 빔으로 trap.

### Formulae

For $^6\text{Li}$, $\Gamma \simeq 2\pi \cdot 6\text{MHz}$, $I_{\text{sat}} \simeq 3\text{mW/cm}^2$

* Gaussian beam intensity profile

$$
I(\rho,z) = \frac{2P}{\pi \text{w}_0^2 (1+z^2/z_R^2)} \exp\left(-\frac{2\rho^2}{\text{w}_0^2 (1+z^2/z_R^2)}\right)
$$

$z$는 빔 진행방향, $P$ 는 빔 파워, $\text{w}_0$는 $1/e^2$ waist radius, $z_R=\pi \text{w}_0/\lambda$는 Rayleigh range.

$k=m\omega^2 = \alpha I^{\prime\prime}$ 이고, beam intensity profile 을 up to second order 까지 전개하는 근사를 취한다면 각각 빔의 radial 방향 $\rho$ 와 빔의 진행방향 $z$ 에 대해

$$
\omega_\rho/2\pi \simeq \sqrt{2\alpha P/\pi^3 m \text{w}_0^4}, \quad \omega_z/2\pi \simeq \sqrt{\alpha P/\pi^3 m \text{w}_0^2 z_R^2}
$$

> typo in MPU: polarizability $\alpha$ 가 생략돼 있는데, dimension 을 체크해보면 $\alpha$ 가 있어야 한다.

예제: $^6\text{Li}$의 경우 $\lambda=1064nm$, focues waist $w_0=25\mu m$, $P=100mW$ 일때 만들어지는 트랩은 $\omega_\rho /2\pi \simeq 1.2\text{kHz}$, $\omega_\rho/\omega_z = \sqrt{2}\pi \text{w}_0/\lambda \simeq 100$.

* $CO_2$ laser 같은 걸로 $\lambda=10.6\mu m$ 처럼 resonance 에서 엄청 먼 빔을 쏘면 Quasi-electrostatic trap (QUEST) 를 만들 수 있음.

* crossed-dipole trap: 다이폴 트랩을 두개쓰면 더 구형대칭에 가까운 트랩을 만들 수 있지만 트랩 볼륨은 줄어듬.

## Hybrid trap

* Cylindrial symmetry 는 vortex 생성에 중요함(ref: Vortices and superfluidity in a strongly interacting Fermi gas of cold atoms, Nature, 435 1047-1051).

* 마그네틱 코일을 Helmholtz 구성의 코일보다 더 멀리 떨어진 두 코일을 ODT axial 방향으로 배치하면 low field seeker 를 위한 트랩으로 쓸 수 있음. (why?)

* 또는 마그네틱 코일을 Helmholtz 구성의 코일보다 가깝게(distance equals radius) high field seeker 를 위한 트랩으로 쓸 수 있음. (why?)

* 결과적으로 ODT 진행방향에 radial 하게는 optical trap, axial 하게는 magnetic trap 을 쓰는 hybrid trap 이 가능. 자세한 것은 2.4.1.

### Compensation of gravity

중력에 의한 potential $-mgx$와 마그네틱 트랩에 의한 포텐셜을 고려하면, ODT 를 magnetic trap 의 센터에 가져다 맞추는게 아니라 약간 더 위의 sweet spot 에 갖다 두는게 좋음. 

ODT 가 sweet spot 에 없다면 10ms 정도 ToF expansion 했을때 아톰이 특정방향으로 새는게 보임. 그걸 막는 방향으로 ODT 를 정렬해야함.

### Trap depth and beam waist

trap depth $U$ 가 $E_F$ 보다 많이 크지는 않는게 냉각 효율이 좋음.

For harmonic trap,

$$
E_F = \hbar(\omega_r^2\omega_z)^{1/3}(3N)^{1/3}
$$

$$
U = \frac{1}{4}m\omega_r^2\text{w}_0^2
$$

$U\ge E_F$ 이므로, 최소한의 waist $\text{w}$ 를 구할 수 있다.

자기장을 높이는 식으로 trap frequency 를 올리는 것은 어려움. 코일의 전류를 올리면 손실되는 전력은 제곱배가 되기 때문.

## Questions

* Fermion 이 Boson 보다 숫자가 많으면 냉각효율 떨어짐 (why?).

* DFG 의 경우 Fermi sea 에서의 hole excitation 때문에 background gas collision 같은 로스에 더 취약하다고 한다(why? ref: Degenerate Fermion Gas Heating by Hole Creation)

* 마그네틱 코일을 Helmholtz 구성의 코일보다 더 멀리 떨어진 두 코일을 ODT axial 방향으로 배치하면 low field seeker 를 위한 트랩으로 쓸 수 있음. (why?)

* 또는 마그네틱 코일을 Helmholtz 구성의 코일보다 가깝게(distance equals radius) high field seeker 를 위한 트랩으로 쓸 수 있음. (why?)
