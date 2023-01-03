optical clock 은 원자의 transition frequency $\nu_0$ 를 이용하는 것인데, 외부의 perturbation 에도 변화없이(low $\triangle \nu$) 안정적인 것이 좋은 시계다.

fractional instability 는 Allan deviation 으로 주어지는데

$$
\sigma_y(\tau)\simeq \triangle \nu/(\nu_0\sqrt{N\tau})
$$

여기서 $\tau$ 는 총 관측시간이고, N은 oscillator 의 총 갯수(원자가 됐든 이온이 됐든)이다. transition 진동수는 높은데 진동수의 변화는 적고, 또 시스템 원자의 갯수는 많고, 관측 시간이 길수록 instability 가 적은 안정적인 시계가 된다. 

ion 의 경우 Coulomb 상호작용이 강하기 때문에 트랩 하나당 single ion 정도밖에 쓸수 없고, 이런 제약이 fractional instability 에서 N 값을 작게 만든다.

중성원자의 경우 원자끼리의 상호작용이 훨씬 약한데, optical lattice 를 이용해서 중성원자들을 격자에 붙잡아 둘 수 있다. 

laser 를 이용해 spatial interference 패턴을 optical wavelength $\lambda_L$ 보다 작게 만들 수 있고, 원자들을 submicrometer 영역에 붙잡아 둘 수 있게된다. 

lattice laser 에 노출된 원자들은 외부 perturbation 에 노출된 것이므로 transition frequency 가 변하는 light shift 를 겪게 되는데, 세기가 I 인데 lattice laser 에 노출된 원자의 transition frequncy 는 다음과 같다.

$$
\nu(\lambda_L,e) = \nu_0+\nu_{ac}= \nu_0 - \frac{\triangle \alpha(\lambda_L,e)}{2\epsilon_0 ch}+O(I^2)
$$

여기서 $\epsilon_0$는 free space 의 permittivity 이고, $\triangle \alpha(\lambda_L,e) = \alpha_u - \alpha_d$ 는 upper state 와 lower state 의 a.c. polarizabilities 의 차이이다.

$O(I^2)$ 이 무시할만큼 작다면, $\triangle \alpha(\lambda_L,e)=0$ 이 되게끔 하는 $\lambda_L$ 을 찾으면 $\nu \simeq \nu_0$ 가 되게 할 수 있다(frequency 나 wavelength 를 측정하는게 I나 polarizability $e$를 측정하는것보다 쉬워서 $\lambda_L$을 찾는다).


## ref 

[An optical lattice clock, M.Takamoto, H.Katori et al, Nature, 435, 321-324 (2005)](https://www.nature.com/articles/nature03541)
