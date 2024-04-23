Gross-Pitaevskii 방정식은 nonlinear equation 인데, 방정식을 풀기 위해서 kinetic energy term 을 무시하는 approximation.

$$
\left(-\frac{\hbar^2}{2m}\nabla^2  +V(\bold{r}) +U_0 |\psi(\bold{r})|^2 \right)\psi(\bold{r})=\mu \psi(\bold{r})
$$

BEC 가 harmonic trap 에 담겨 있는 상황을 가정해보자.

원자 구름의 사이즈를 $\xi$ 라고 한다면, 

$$
E_{\text{kinetic}}\sim \frac{\hbar^2}{2m\xi^2}
$$

$$
V\sim \frac{m \omega_0^2}{2}\xi^2
$$

kinetic energy 와 potential 에너지가 비례한다고 가정하면(virial theorem), $E_{\text{kinetic}} = V$ 이므로

$$
\xi = \sqrt{\frac{\hbar}{m\omega_0}}
$$

로 쓸 수 있다.

각 입자별 평균 interaction energy 는

$$
E_{\text{int}}\sim U_0 n
$$

이때 kinetic energy 와 interaction energy 둘 다 원자구름을 expand 하는 방향의 힘이므로, $U_0$ 가 특정 값 $U_0^{\text{crit}}$ 보다 크다면 상대적으로 더 작은 값인 kinetic term 을 무시할 수 있다.

$$
U_0^{\text{crit}}\sim \frac{\hbar \omega_0}{2n}
$$

Schrodinger 방정식에서 kinetic term 을 무시하면,

$$
\mu \psi \simeq \left(V + U_0 |\psi|^2\right)\psi
$$

$$
|\psi(\bold{r})|^2 = n(\bold{r}) =\begin{cases}
\frac{\mu -V(\bold{r})}{U_0} & \text{for r such that } \frac{\mu -V(\bold{r})}{U_0}\\
0 & \text{otherwise}
\end{cases}
$$

Thomas-Fermi 근사가 성립하려면 

$$
U_0 n \gg \frac{\hbar\omega_0}{2}
$$
이고, $U_0n$ 이 harmonic oscillator 의 ground energy 보다 훨씬 크므로 $V+U_0 n=\mu$ 에서 $U_0 n\sim \mu$ 라고 쓸 수 있다.

$n\sim N/R^3$, 이때 $R$ 은 $V(R)=\mu$ 가 되는 지점이라고 할때, 

$$
\frac{1}{2}m\omega_0^2 R^2 = \mu
$$

$$
R = \sqrt{\frac{2\mu}{m\omega_0}}
$$

따라서 
$$
N \sim R^3\frac{\mu}{U_0} = \left(\frac{2}{m\omega_0}\right)^{3/2}\frac{1}{U_0}\mu^{5/2}
$$

$$
\mu \sim N^{2/5} \quad\text{in harmonic trap}
$$

라고 할 수 있다.