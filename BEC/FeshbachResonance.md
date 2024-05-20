## Scattering resonance



## Feshbach resonance

Feshbach resonance: 두 원자의 collision cross-section 이 엄청나게 커지는 현상 when open channel의 스캐터링 continuum 과 closed channel 의 bound state 가 교차할 때.

자기장 $B$ 에 따른 effective scattering length 는 다음과 같다.

$$
a(B) = a_{BG}\left[ 1-\frac{\triangle B}{B-B_0} \right]
$$

$a_{BG}$ 는 오픈채널과 클로즈채널 사이의 커플링이 없을 때의 scattering length 이고, $B_0$ 와 $\triangle B$ 는 각각 resonance 위치와 width 이다.

일반적으로 $a_{BG}>0$, $\triangle B>0$ 이므로 $B$ 가 커질수록 scattering length $a$ 는 절댓값이 작아지는 음수이므로, 실험 결과를 보여줄때 $1/k_Fa$ 대신 $-1/k_Fa$ 를 축으로 그래프를 그린다.

Feshbach resonance:
two fermions in the “open channel” coupled to a bound state in the “closed channel”.
However, essentially all crossover experiments are in the so-called ‘broad’ Feshbach
resonance limit where the width of the resonance is much larger than the Fermi energy.
In this limit, an effective single-channel model is sufficient [1]

$l=0$ 인 s-wave 상황에서 electron spin-nuclear spin 의 hyperfine interaction 은 다음과 같다.

$$
V_{hf} = \frac{a_{hf}}{\hbar^2}(\hat{S}_1 \cdot \hat{I}_1+\hat{S}_2 \cdot \hat{I}_2) \\= \frac{a_{hf}}{2\hbar^2}(\hat{S}_1+\hat{S}_2)\cdot(\hat{I}_1+\hat{I}_2) + \frac{a_{hf}}{2\hbar^2}(\hat{S}_1-\hat{S}_2)\cdot(\hat{I}_1-\hat{I}_2) 
= V^+_{hf} + V^-_{hf}
$$

이때 $\hat{S}_1+\hat{S}_2 = \hat{S}$ 이므로, $V^+_{hf}$는 electron spin singlet ($S=0$) 과 electron spin triplet ($S=1$) 에 대해 diagonalize 돼 있지만, $V^-_{hf}\sim\hat{S}_1-\hat{S}_2$ 가 off-diagonal 이므로, singlet 과 triplet 사이에 커플링을 만든다.

(Fermionic Feshbach molecular gas 의 경우 bosonic gas와는 다르게 Feshbach resonance 근처에서 안정적이다. Li6 의 경우 10s 정도로 길다. Why? inelastic collision, 즉 three-body collision 을 하려면 일정 영역에 Fermion 3개가 모여야 되는데, 3개가 모인다면 그 중 2개는 반드시 같은 방향 스핀일 것이므로 3개가 동시에 모이기가 힘들다.)


## Ref

[1] BEC-BCS crossover 

MPU chapter 5