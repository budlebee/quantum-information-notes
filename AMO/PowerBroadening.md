# Power broadening

Homogeneous broadening. 모든 원자가 동일하게 겪는 broadening.

원자에 쏘는 빛의 세기가 강해져도 absorption peak 의 높이는 saturation 되고, peak 이 넓게 퍼지는 현상. Atomic oscillator 가 saturation 돼서 그렇다.

바닥상태는 decay 가 없고, 여기상태는 purely decay 하는 ($\Gamma_t=\Gamma_0$) 2-level system density matrix 의 equation of motion은 다음과 같다.

$$
\dot{\rho}_{aa}=-\Gamma_0 \rho_{aa} + \frac{i}{2}\Omega e^{-i\omega t}\rho_{ba} +c.c. \\
\dot{\rho}_{ab} = -\gamma\rho_{ab} - i\omega_0 \rho_{ab}-\frac{i}{2}\Omega e^{-i\omega t}(\rho_{aa}-\rho_{bb})
$$

여기서 $\gamma=\Gamma/2$ 이다.

시스템이 saturation 된 steady state 라면, $\dot{\rho}_{aa}=\dot{\rho}_{bb}=0$ 이고, $\rho_{ab}$ 는 external driving frequency 에 따라 움직일 것이므로 $\dot{\rho_{ab}}=-i\omega\rho_{ab}$ 이다.

> note: mathematical trick
>$$
>\rho_{ab} = (\sigma_1+i\sigma_2)e^{-i\omega t}\\
>\rho_{aa}-\rho_{bb} = \sigma_3
>$$
>
>위와 같이 정의한 다음 실수부분과 복소수 부분을 나눠서 방정식을 풀면 답을 얻을 수 있다.

이때 

$$
\Omega^2 = \frac{\mu^2 E_0^2}{\hbar^2} =\frac{1}{\hbar\omega} \frac{6\pi^2c^2}{\omega_0^2}\frac{4\mu^2\omega_0^3}{3\hbar c^3}\frac{cE^2_0}{8\pi}= \frac{\sigma_{rad}\Gamma_0 I_0}{\hbar \omega_0}
$$

또한 $I_s$ 라는 saturation intensity 를 정의해 줄 수 있는데, 정의는 다음과 같다.

$$
I_{s} = \frac{\hbar \omega}{2\sigma_{rad} (2\gamma)^{-1}} = \frac{\textnormal{single photon energy}}{2(\textnormal{cross-section})(\textnormal{dephasing time})}
$$

따라서

$$
\rho_{ab} = \frac{\Omega(-(\omega-\omega_0)+i\gamma)/2}{(\omega-\omega_0)^2+\gamma^2(1+I_0/I_s)}e^{-i\omega t}\\
\rho_{aa} = \frac{\gamma^2(I_0/I_s)/2}{(\omega-\omega_0)^2 + \gamma^2 (1+I_0/I_s)}
$$

absorption spectrum 의 y축 값은 $rho_{aa}$에 비례하므로, $\rho_{aa}$ 가 1/2이 되는 $\omega_{FWHM}$ 을 계산해서 bandwidth 를 구하면 다음과 같다.

$$
\triangle \omega_{FWHM} = 2\gamma\sqrt{1+I_0/I_s}
$$

들어오는 빛의 세기 $I_0$ 가 강할수록 FWHM 이 넓어진다. 또한 $\rho_{aa}$ 는 1/2 로 saturation 된다.

> note: Uncertainty 관점에서 파워 브로드닝 생각해보기 (possible?).
