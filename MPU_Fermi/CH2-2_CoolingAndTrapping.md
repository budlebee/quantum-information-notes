

laser cooling & magnetic trapping: boson 이랑 똑같음.

## Sympathetic cooling

두종류의 원자를 쓰기 때문에 질량이 달라서 중력에 의한 영향이 다름. 루비듐-리튬 처럼 질량차이가 큰 경우 특히 심함.

하모닉 트랩에서 수직방향으로 생기는 sag는 

$$
\triangle x = \frac{g}{\omega^2}
$$

sag 를 줄이려면 트랩 프리퀀시를 올려야 하지만 그러면 three-body loss 가 심해짐.

Fermion 이 Boson 보다 숫자가 많으면 냉각효율 떨어짐.

DFG 의 경우 Fermi sea 에서의 hole excitation 때문에 background gas collision 같은 로스에 더 취약하다고 한다(why? ref: Degenerate Fermion Gas Heating by Hole Creation)

BEC 의 heat capacity 는 0에 가깝지만, 아주 낮은 온도라서 일반적인 Bose 가스보다 더 Fermion 샘플을 냉각할 수 있다.

Intraspecies scattering length: attractive 하거나 repulsive 하거나. Bose gas 에 의한 attractive 상호작용은 많은 Fermion 들을 한데 뭉치게 해서 heating 과 loss 로 이어질 수 있다 (ref: Collapse of a degenerate Fermi gas, Science, 297 2240).

RF 펄스와 decoherence 를 이용해 two-components mixture 를 만들면 maximu, occupation 이 1/2 이 되고 effective $T/T_F$ 가 0.6이 되기 때문에, 그 아래로 냉각하는 것은 별 이득이 없다 (section 2.3.5 참고).

## Optical trap

AC Stark shift 를 이용한 trapping: 스핀 상태에 상관없이 붙잡을 수 있음.

High power laser 와 enhancement cavity 를 다룰 수 있다면 Magnetic trap 없이 all-optical trap 도 가능. $^6\text{Li}$의 경우 마그네틱 트랩을 안쓴다면 다른 원자를 쓸 필요가 없다.

red detune 된 가우시안 빔으로 trap.

### Formulae

For $^6\text{Li}$, $\Gamma = 2\pi \cdot 6\text{MHz}$, $I_{\text{sat}} = 3\text{mW/cm}^2$

* Gaussian beam intensity profile

$$
I(\rho,z) = \frac{2P}{\pi \text{w}_0^2 (1+z^2/z_R^2)} \exp\left(-\frac{2\rho^2}{\text{w}_0^2 (1+z^2/z_R^2)}\right)
$$

$z$는 빔 진행방향, $P$ 는 빔 파워, $\text{w}$는 $1/e^2$ waist radius, $z_R=\pi \text{w}_0/\lambda$는 Rayleigh range.

Dipole trap 의 바닥 근방은 harmonic trap 으로 근사 가능.

$$
\omega_\rho/2\pi \simeq \sqrt{2P/\pi^3 m \text{w}_0^4}, \quad \omega_z/2\pi \simeq \sqrt{P/\pi^3 m \text{w}_0^2 z_R^2}
$$

예제: $^6\text{Li}$의 경우 $\lambda=1064nm$, focues waist $w_0=25\mu m$, $P=100mW$ 일때 만들어지는 트랩은 $\omega_\rho /2\pi \simeq 1.2\text{kHz}$, $\omega_\rho/\omega_z = \sqrt{2}\pi \text{w}_0/\lambda \simeq 100$.

아예 $CO_2$ laser 같은 걸로 $\lambda=10.6\mu m$ 처럼 resonance 에서 엄청 먼 빔을 쏘면 Quasi-electrostatic trap (QUEST) 를 만들 수 있음.

crossed-dipole trap: 다이폴 트랩을 두개쓰면 더 구형대칭에 가까운 트랩을 만들 수 있지만 트랩 볼륨은 줄어듬.

## Hybrid trap

Cylindrial symmetry 는 vortex 생성에 중요함(ref: Vortices and superfluidity in a strongly interacting Fermi gas of cold atoms, Nature, 435 1047-1051).

마그네틱 코일을 Helmholtz 구성의 코일보다 더 멀리 떨어진 두 코일을 ODT axial 방향으로 배치하면 low field seeker 를 위한 트랩으로 쓸 수 있음.

또는 마그네틱 코일을 Helmholtz 구성의 코일보다 가깝게(distance equals radius) high field seeker 를 위한 트랩으로 쓸 수 있음.

결과적으로 ODT 진행방향에 radial 하게는 optical trap, axial 하게는 magnetic trap 을 쓰는 hybrid trap 이 가능. 자세한 것은 2.4.1.

### Compensation of gravity

중력에 의한 potentail $-mgx$와 마그네틱 트랩에 의한 포텐셜을 고려하면, ODT 를 magnetic trap 의 센터에 가져다 맞추는게 아니라 약간 더 위의 sweet spot 에 갖다 두는게 좋음. Gravity shifts the saddle potential by an amount $2g/\omega_z^2$.

Anti-confining curvatyre $i\omega_z/\sqrt{2}$ (why? Iofe 트랩이라서 그런가?)

ODT 가 sweet spot 에 없다면 10ms 정도 expansion 했을때 아톰이 특정방향으로 새는게 보임. 그걸 막는 방향으로 ODT 를 정렬해야함.

### Trap depth and beam waist

trap depth $U$ 가 $E_F$ 보다 많이 크지는 않는게 냉각 효율이 좋음(why?).

For harmonic trap,

$$
E_F = \hbar(\omega_r^2\omega_z)^{1/3}(3N)^{1/3}
$$

$$
U = \frac{1}{4}m\omega_r^2\text{w}_0^2
$$

$U\ge E_F$ 이므로, 최소한의 waist $\text{w}$ 를 구할 수 있다.

$\omega_z$ 를 높이는 것은 어려움. 코일의 전류를 올리면 손실되는 전력은 제곱배가 되기 때문.


## Questions

* DFG 의 경우 Fermi sea 에서의 hole excitation 때문에 background gas collision 같은 로스에 더 취약하다고 한다(why? ref: Degenerate Fermion Gas Heating by Hole Creation)

* Anti-confining curvatyre $i\omega_z/\sqrt{2}$ (why? Iofe 트랩이라서 그런가?)

* trap depth $U$ 가 $E_F$ 보다 많이 크지는 않는게 냉각 효율이 좋음(why?).