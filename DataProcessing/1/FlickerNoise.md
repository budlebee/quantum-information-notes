
1/f noise 라고 불리는 노이즈. 1/f^a 형태로 주파수에 따라 노이즈의 세기가 변한다. a 가 1이면 pink noise 라고 부른다.

## $1/f^{a}$ from the superposition of relaxation processes

$t=0$ 인 시점에 켜지고 $\lambda$로 relaxation 하는 신호 $N(t)=N_0 e^{-\lambda t}$ 를 생각해보자. 해당 신호의 Fourier transform 은

$$
\begin{aligned}
F(\omega) &= \int_{-\infty}^{\infty} N(t)e^{-i\omega t}dt \\
&= \int_{-\infty}^{\infty} N_0 e^{-\lambda t}e^{i\omega t}dt \\
&= N_0 \int_{-\infty}^{\infty} e^{-(\lambda-i\omega)t}dt \\
&= N_0 \frac{1}{\lambda+i\omega}
\end{aligned}
$$

이와 같은 펄스가 여러번 이어지는 펄스 트레인은 $N(t,t_k) = N_0 e^{-\lambda(t-t_k)}$ 의 합인데 이를 Fourier transform 하면
$$
F(\omega) = \int_{-\infty}^{\infty} \sum_{k} N(t,t_k)e^{-i\omega t}dt = N_0 \sum_{k} \frac{1}{\lambda+i\omega}e^{i\omega t_k}
$$

해당하는 함수의 power spectrum $S(\omega)$는
$$
S(\omega) =\lim_{T\to \infty}\frac{1}{T} \langle|F(\omega)|^2\rangle =\frac{N_0^2}{\lambda^2 + \omega^2} \lim_{T\to \infty}\frac{1}{T} \langle |\sum_k e^{i\omega t_k} |^2\rangle= \frac{N_0^2 n}{\lambda^2 + \omega^2}
$$

0점 근처에서는 saturation 된 커브를, 먼 곳에서는 $1/\omega^2$ 에 비례하는 커브를 볼 수 있다. 이는 $1/f^2$ 형태의 power spectrum 을 가지는 것이다.


## Ref

- 1/f noise: a pedagogical review, Edoardo Milotti.