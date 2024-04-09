
## Density and momentum distribution of BEC in 3D harmonic trap

Absortion image 로 BEC cloud 의 분포를 측정한다. 

샘플이 잡히자 마자 in-situ 로 이미징을 하면 density profile 을 알 수 있고, trap potential 을 꺼서 cloud 를 팽창시킨뒤에 이미징을 하면 momentum distribution 을 알 수 있다 (Time of Flight, ToF). 

Trapping angular frequency  $\omega_x$, $\omega_y$, $\omega_z$ 인 경우 $V(\bold{r})=m(\omega_x^2 x^2 + \omega_y^2 y^2 +\omega_z^2 z^2)/2$ 이고, 모든 원자들이 non-interacting 한 경우에는 density distribution $n(\bold{r})$을 single particle wavefunction $\phi_0 (\bold{r})$로 쓸 수 있다.

$$
n(\bold{r}) = N|\phi_0 (\bold{r})|^2
$$

3D harmonic oscillator 에 대한 wavefunction solution $\phi_0(\bold{r})$ 은 다음과 같다.

$$
\phi_0(\bold{r}) = \frac{1}{\pi^{3/4}\sqrt{a_x a_y a_z}} e^{-(x^2/2a_x^2+y^2/2a_y^2+z^2/2a_z^2)}
$$

where $a_i=\sqrt{\hbar/m\omega_i}$.

해당 솔루션을 Fourier transform 하면 모멘텀 분포를 얻을 수 있다.

$$
\phi_0(\bold{p}) = \frac{1}{\pi^{3/4}\sqrt{c_x c_y c_z}} e^{-(p_x^2/2c_x^2+p_y^2/2c_y^2+p_z^2/2c_z^2)}
$$

where $c_i=\hbar/a_i=\sqrt{m\hbar\omega_i}$.

#### anisotropic 한 포텐셜에서는 anisotropic 한 momentum distribution 을 가지는 반면, $T \gg T_c$ 인 thermal gas 의 경우 anisotropic 한 포텐셜에서도 isotropic 한 momentum distribution 을 가진다.

$$
n_{th}(\bold{r}) = \frac{N}{\pi^{3/2}{R_x R_y R_z}} e^{-(x^2/2R_x^2 + y^2/2R_y^2+z^2/2R_z^2)}
$$

where $R_i=\sqrt{2k_B T /mw_i^2}$, and

$$
n_{th}(\bold{p}) \sim  e^{-p^2/2mk_B T}
$$

따라서 BEC 가스와 thermal gas 는 충분히 긴 ToF 시켰을때 서로 다른 양상을 보인다. 