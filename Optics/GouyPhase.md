# Gouy Phase

focusing 지점이 $z=0$ 인, $z$ 방향으로 날아가는 빔에서 z 방향 phase 가 생기는 현상.

![gaussian-beam-propagation-fig-2](./img/gaussian-beam-propagation-fig-2.png)

 $z=-\infty$ 에서 $z=\infty$ 까지 날아가면 z 방향 phase shift 가 생겨나는 것. Spherical beam 의 경우 $\pi$ 만큼, Cylidrical beam 의 경우 $\pi/2$ 만큼 phase shift $\phi_G$ 가 생긴다.

이런 phase shift 가 일어나는 이유는 진행방향과 다른 wave vector $k_x$ 와 $k_y$ 들로 인해 effective propagation wave vector $\bar{k_z}$ 가 줄어드는 것 때문에 생긴다.

즉, Gouy shift 는 transverse momentum spread 때문에 생기는 axial phase shift 다.

Gouy phase $\phi_G$ 를 다음과 같이 쓸 수 있다.

$$
\phi_G = -\frac{1}{k}\int^z (\langle k_x^2 \rangle +\langle k_y^2 \rangle)dz
$$

beam 의 공간적인 normalized $x,y$ distribution function 을 $f(x,y)$, wave momentum 의 normalized distribution function 을 $\tilde{F}(k_x,k_y)$ 라고 한다면, 

$$
\tilde{F}(k_x,k_y) = \frac{1}{2\pi}\int_{-\infty}^{\infty}\int_{-\infty}^{\infty} f(x,y)e^{-ik_xx-ik_yy}dxdy
$$

공간적인 분포를 Gaussian beam 으로 생각한다면, 

$$
f(x,y) = \sqrt{\frac{2}{\pi}}\frac{1}{w(z)}\exp{[\frac{x^2+y^2}{w^2(z)}]}
$$
where
$$
w^2(z) = w_0^2[1+\frac{z^2}{z_R^2}]\\
z_R = \frac{\pi w_0^2}{\lambda}
$$
이 된다.

모멘텀 벡터 제곱의 기댓값은
$$
\langle k_x^2 \rangle = \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} k_x^2 |\tilde{F}(k_x,k_y)|^2 dk_x dk_y \\
= \frac{1}{w^2(z)}=\langle k_x^2 \rangle 
$$

이므로, Gouy phase 는 다음과 같이 쓸 수 있다.

$$
\phi_G = -\frac{1}{k}\int^z (\langle k_x^2 \rangle +\langle k_y^2 \rangle)dz = -\frac{n}{k}\int^z \frac{1}{ w^2(z)}dz
$$
이때 cylindrical wave는 transverse 모멘텀중 하나의 기여가 없을 것이므로 n=1, spherical wave 는 n=2 이다.

결과적으로 

$$
\phi_G = -\frac{n}{2}\arctan{(z/z_R)}
$$ 

가 돼서,  $z=-\infty$ 에서 $z=\infty$ 까지 날아가면 z 방향으로 spherical beam 은$\pi$ 만큼, cylindrical beam 은 $\pi/2$ 만큼  phase shift 가 생긴다.


이런 Gouy phase 는 zeroth order Gaussian beam 뿐만 아니라, higher-order Hermite-Gaussian beam 에서도 위와 비슷한 방식으로 유도할 수 있다.

## ref

Physical origin of the Gouy phase shift, Simin Feng, Herbert G, Winful, Optics Letters, Vol. 26, No. 8, April 15, 2001
