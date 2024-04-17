

## Grand canonical ensemble

* canonical ensemble: system 과 reservoir 가 열교환만 함(particle 교환은 X)

* grand canonical ensemble: system 과 reservoir 가 열과 particle을 교환함. 이 경우 시스템은 온도 $T$ 와 chemical potential $\mu = (\partial E/\partial N)_{S,V}$ 로 결정됨.

### Bose-Einstein distribution

$$
f_{BE}(\epsilon_\nu) = \langle n\rangle = \frac{1}{e^{(\epsilon_\nu-\mu)/k_B T}-1}
$$

mean particle number $N$
$$
N = \sum_{\nu} f_{BE}(\epsilon_\nu)
$$

mean energy $E$
$$
E= \sum_{\nu} \epsilon_\nu f_{BE}(\epsilon_\nu) 
$$

Approximation: summation to integral 

$$
N = \sum_{\nu} f_{BE}(\epsilon_\nu) \simeq \int_0^{\infty} d\epsilon f(\epsilon) g(\epsilon)
$$

이때 $g(\epsilon)= d G(\epsilon)/d \epsilon$ 인 density of states ($G(\epsilon)$은 $\epsilon$ 이하 에너지의 입자들의 total number of states).

> Note: Density of state 가 작다면 summation 을 integral 로 바꾼 approximation 은 유효하지 않으니까 주의.

### Density of state in 3D

In quantized space, unit real space volume is V=$L_x L_y L_z$. By the periodic boundary condition, $k_i=2\pi/L_i$

$k$ 벡터가 위상공간에서 차지하는 공간 $4\pi k^3/3$을 unit phase space volume 으로 나눠주면, 에너지가 $\epsilon = \hbar k/2m$ 이하의 Boson 들의 total number of states 를 구할 수 있다.

$$
G(\epsilon) = \frac{4\pi k^3/3}{(2\pi/L)^3} = V\frac{\sqrt{2}}{3\pi^3 \hbar^3}(m\epsilon)^{3/2}
$$

The density of states $g(\epsilon)$

$$
g(\epsilon) = \frac{d G(\epsilon)}{d\epsilon} = V\frac{1}{\sqrt{2}\pi^2 \hbar^3}m^{3/2}\epsilon^{1/2}
$$

일반적으로 denisty of states 는 $g(\epsilon)=C_{\alpha}\epsilon^{\alpha-1}$ 의 형태로 표시하며, homogeneous box trap 의 경우 d dimension 에 대해 $\alpha=d/2$ 이고, harmonic trap 의 경우 $\alpha=d$ 이다.

### Density of states in 3D harmonic trap

3D simple harmonic oscillator 의 에너지는

$$
\epsilon = (\frac{1}{2}+n_x)\hbar \omega_x +(\frac{1}{2}+n_y)\hbar \omega_y+(\frac{1}{2}+n_z)\hbar \omega_z
$$

에너지가 $\hbar\omega_i$ 에 비해 커서 zero-point 에너지를 무시할 수 있다면, $\epsilon_i=\hbar\omega_i$ 이고 $\epsilon = \epsilon_x+\epsilon_y+\epsilon_z$ 이므로 total number of states 는 다음과 같이 쓸 수 있다.

$$
G(\epsilon) =\frac{\text{total energy}}{\text{unit energy volume}}=\frac{1}{(\hbar\omega_x)(\hbar\omega_y)(\hbar\omega_z)}\int_0^\epsilon d\epsilon_x \int_0^{\epsilon-\epsilon_x} d\epsilon_y \int_0^{\epsilon-\epsilon_x-\epsilon_y} d\epsilon_z = \frac{\epsilon^3}{6\hbar^3\omega_x\omega_y\omega_z}
$$

$$
g(\epsilon) = \frac{\epsilon^2}{2\hbar^3 \omega_x\omega_y\omega_z}
$$

d-dimension 에 대해 일반화 하면, 

$$
g(\epsilon) = \frac{\epsilon^{d-1}}{(d-1)! \prod_i \hbar\omega_i}
$$

## Bose-Einstein Condensation and condensation fraction

Bose-Einstein 분포에서 chemical potential $\mu$는 negative value 이고(positive 라면 occupation 이 음수라는 unphysical 한 결과가 나온다), 시스템의 밀도를 높일수록 chemical potential 이 커져서 0에 도달하게 된다.

$\mu=0$ 일때 $\epsilon >0$ 인 excited states 의 숫자 $N_{ex}$ 는 다음과 같다.

$$
N_{ex}(\mu=0) = C_{\alpha}\int_0^\infty d\epsilon \frac{\epsilon^{\alpha-1}}{e^{\epsilon/k_B T}-1}
$$

이때 Gamma function $\Gamma(\alpha)$와 Riemann zeta function $\zeta (\alpha)$ 에 대해서
$$
\int_0^\infty dx \frac{x^{\alpha-1}}{e^x-1} = \Gamma(\alpha)\zeta(\alpha)
$$ 

이므로, 

$$
N_{ex}(\mu=0) = C_{\alpha}\int_0^\infty d\epsilon \frac{\epsilon^{\alpha-1}}{e^{\epsilon/k_B T}-1} = C_\alpha \Gamma(\alpha)\zeta(\alpha)(k_B T)^\alpha
$$

excited state 의 갯수가 제한되고 나머지 모든 입자는 ground state 로 가게 된다 (Bose-Einstein condensation).

이때 모든 입자들이 excited state 에 있는 상태를 $T_c$ 로 정의하면, 이 경우 

$$
N=N_c=C_\alpha \Gamma(\alpha)\zeta(\alpha)(k_B T_c)^\alpha
$$

가 된다.

$T_c$ 아래에서는 $N=N_0+N_{ex}$ 이므로, 전체 중 condensation 부분인 $N_0$ 를 구하면

$$
N_0 = N-N_{ex} = N\left[1-\left(\frac{T}{T_c}\right)^\alpha\right]
$$

### Critical density and thermal de-Broglie wavelength

3D homogeneous trap 에서 $\alpha=3/2$ 이고 $\Gamma(3/2)\zeta(3/2)\simeq 2.3$ 인데, 이때 critical density $n_c=N/V$ 를 thermal de-Broglie wavelength $\lambda_T = \sqrt{2\pi \hbar^2 / mk_B T}$ 로 나타내면 다음과 같다.

$$
n_c \simeq 2.3 \frac{m^{3/2}}{\sqrt{2}\pi^2 \hbar^3}(k_B T)^{3/2} \simeq 2.6 \frac{1}{\lambda_T^3}
$$
