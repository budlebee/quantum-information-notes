
## Feshbach resonance

- 일반적인 실험 환경의 알칼리 아톰들은 다른 open channel 들의 효과가 작아서 scattering length 가 real number 인 single-channel scattering theory 로 근사가 가능하다.
- Feshbach resonance 는 한 채널의 Elastic scattering 이 low-energy bound state 가 있는 다른 채널로 dramatically 교체되는 현상 (Pethick ch 5.4.2)
- 오픈채널의 total energy 가 클로즈채널의 bound state 에너지와 일치할때 발생한다.

### Basic formalism

- Wave function of spatial and spin degree freedom $|\Psi\rangle = |\Psi_P\rangle + |\Psi_Q\rangle$ where $|\Psi_P\rangle \equiv \hat{P}|\Psi\rangle$ and $|\Psi_Q\rangle \equiv \hat{Q}|\Psi\rangle$
- $P$ : subspace of open channel / $Q$ : subspace of closed channel.
- $\hat{P}$, $\hat{Q}$ : projection operators for open and closed channel. $\hat{P}+\hat{Q}=1$, $\hat{P}\hat{Q}=0$.
- $\hat{P}\hat{P}=\hat{P}$, $\hat{Q}\hat{Q}=\hat{Q}$ 이므로, $\hat{H}|\Psi\rangle=E|\Psi\rangle$ 에 대해
$$
(E-PHP)|\Psi_P\rangle =PHQ|\Psi_Q\rangle \rightarrow (E-H_{PP})|\Psi_P\rangle = H_{PQ}|\Psi_Q\rangle  
$$
$$
(E-QHQ)|\Psi_Q\rangle =QHP|\Psi_P\rangle \rightarrow (E-H_{QQ})|\Psi_Q\rangle = H_{QP}|\Psi_P\rangle
$$
- $H_{PP}$ 와 $H_{QQ}$ 는 각 서브스페이스의 해밀토니안, $H_{PQ}$ 와 $H_{QP}$ 는 두 서브스페이스 간의 커플링을 의미한다.
- 여기서, scattering matrix 를 계산하기 위한 positive infinitesimal imaginary part $\delta$ 를 추가하면(J.J.Sakurai chapter 6, Lippmann-Schwinger equation 참고)
$$
|\Psi_Q\rangle = (E-H_{QQ}+i\delta)^{-1}H_{QP}|\Psi_P\rangle
$$
$$
(E-H_{PP}-H'_{PP})|\Psi_P\rangle = 0
$$
where 
$$
H'_{PP}=H_{PQ}(E-H_{QQ}+i\delta)^{-1}H_{QP}.
$$
- 이것이 Feshbach resonance 에 해당하는 텀. P subspace 에서 Q subspace 로 갔다가 다시 P subspace 로 돌아오는 transition 을 뜻하는 effective interaction.

### General solution for Feshbach resonance

- relative motion 에 대한 kinetic enrgy 와 hyperfine, Zeeman terms 를 포함한 부분을 $H_0$, 서브스페이스 내의 interaction term 을 $U_1$ 이라고 한다면 편의상 다음과 같이 쓸 수 있다.
$$
H_{PP}=H_0+U_1
$$
$$
U_2\equiv H'_{PP},~~~ U\equiv U_1+U_2
$$
$$
(E-H_0-U)|\Psi_P\rangle=0.
$$
- T-matrix 에 대해 Limmann-Schwinger equation 을 operator 형태로 쓴다면
$$
T=U+UG_0T, ~~~ \text{where}~G_0\equiv (E-H_0+i\delta)^{-1}.
$$

- 위 식에 대한 formal solution 은
$$
T=(1-UG_0)^{-1}U=U(1-G_0 U)^{-1},
$$
$$
T=(E+i\delta-H_0)(E+i\delta-H_0-U)^{-1}U.
$$
- 이때, $T_1\equiv U_1+U_1G_0T_1$ (P subspace 에서 Q subspace 로의 transition 을 무시할때의 T-matrix)를 정의하면
$$
T=T_1+(1-U_1G_0)^{-1}U_2(1-G_0U)^{-1}.
$$
- Relative momenta $k$ 와 $k'$ 인 plane wave states 에 대해 matrix elements 를 구하면
$$
\langle k'|T|k\rangle = \langle k'|T_1|k\rangle + \langle k'|(1-U_1G_0)^{-1}U_2(1-G_0U)^{-1}|k\rangle.
$$
- 이때 
$$
\langle k'| (1-U_1G_0)^{-1} = [(1-G_0^- U_1)^{-1}|k'\rangle]^\dagger \equiv [|k';U_1,-\rangle]^\dagger, ~~\text{where} ~~~ G_0^- \equiv (E-H_0-i\delta)^{-1}.

$$
- 따라서 matrix elements 는 다음과 같다.
$$
\langle k'|T|k\rangle = \langle k'|T_1|k\rangle + \langle k';U_1,-|U_2|k;U,+\rangle.
$$
### Tuning effective interactions

- 이때 $U_2$ 가 매우 작아 first order 까지만 고려하는 approximation 을 취하면, 즉 $U\simeq U_1$ 이라면,
$$
\langle k'|T|k\rangle = \langle k'|T_1|k\rangle + \langle k';U_1,-|U_2|k;U_1,+\rangle.
$$
- 이때 incoming particle 의 relative velocity 가 0이고, 다른 오픈 채널들끼리의 real scattering 을 무시한다면, incoming 또는 outgoing terms 에 $e^{\pm ikr}$ 같은 phase factor 가 붙지 않으므로 둘다 먼 거리에선 $1-a/r$ 처럼 같은 모습을 보여준다.
- incoming wave function $\langle|k';U_1,-|$ 과 outgoing wave function $|k;U_1,+\rangle$ 을 둘다 $|\psi_0\rangle$  로 쓴다면, $U_2$ 에 대한 matrix elements 를 unit operator $I=\sum_n |n\rangle\langle n|$ 를 이용해서 계산하면 다음과 같은 식을 유도할 수 있다.
$$
\frac{4\pi\hbar^2}{m}a = \frac{4\pi \hbar^2}{m}a_{P} + \sum_n \frac{|\langle\psi_n|H_{QP}|\psi_0\rangle|^2}{E_{th}-E_n}
 $$
- 여기서 $a_P$ 는 P 와 Q 채널간의 커플링을 무시했을때의 scattering length 이다.
- 만약 $E_{th}$가 특정 채널의 bound state $E_{res}$ 근처라면, 나머지 채널의 contribution 을 non-resonance scattering length $a_{nr}$ 이라는 값으로 몰아넣을 수 있으므로
$$
\frac{4\pi\hbar^2}{m}a = \frac{4\pi \hbar^2}{m}a_{nr} + \frac{|\langle\psi_{res}|H_{QP}|\psi_0\rangle|^2}{E_{th}-E_{res}}
$$

> Question: incoming 과 outgoing scattering 차이가 없는 이유는 뭘까?


### Magnetic field and scattering length

-  위 식의 denomiator 부분이 특정 자기장 값 $B=B_0$ 에서 0이 된다고 한다면,
$$
E_{th}-E_{res} \simeq (\mu_{res}-\mu_\alpha - \mu_\beta)(B-B_0),~~\text{where}~~~\mu_\alpha=-\frac{\partial \epsilon_\alpha}{\partial B}~~\text{and}~~-\frac{\partial \epsilon_\beta}{\partial B}
$$
- 그리고 오픈채널에 있는 두 아톰의 magnetic moments 는,
$$
-\frac{\partial E_{res}}{\partial B}
$$
- 따라서 자기장에 따른 scattering length 는 다음과 같다.
$$
a= a_{nr}\left(1-\frac{\triangle B}{B-B_0}\right), ~~\text{where}~~ \triangle B = \frac{B}{4\pi\hbar^2a_{nr}}\frac{|\langle\psi_{res}|H_{QP}|\psi_0\rangle|^2}{(\mu_\alpha+\alpha_\beta-\mu_{res})}
$$

#### Coupling between spin-singlet and spin-triplet states

- $l=0$ 인 s-wave 상황에서 electron spin-nuclear spin 의 hyperfine interaction 이 커플링을 만든다.
$$
V_{hf} = \frac{a_{hf}}{\hbar^2}(\hat{S}_1 \cdot \hat{I}_1+\hat{S}_2 \cdot \hat{I}_2) \\= \frac{a_{hf}}{2\hbar^2}(\hat{S}_1+\hat{S}_2)\cdot(\hat{I}_1+\hat{I}_2) + \frac{a_{hf}}{2\hbar^2}(\hat{S}_1-\hat{S}_2)\cdot(\hat{I}_1-\hat{I}_2) 
= V^+_{hf} + V^-_{hf}
$$
- 이때 $\hat{S}_1+\hat{S}_2 = \hat{S}$ 이므로, $V^+_{hf}$는 electron spin singlet ($S=0$) 과 electron spin triplet ($S=1$) 에 대해 diagonalize 돼 있지만, $V^-_{hf}\sim\hat{S}_1-\hat{S}_2$ 가 off-diagonal 이므로, singlet 과 triplet 사이에 커플링을 만든다.


### Loss near Feshbach resonance

- Near a Feshbach resonance, inelastic loss is strongly enhanced.
- Since the Feshbach bound states have strong couplings to inelastic outgoing channels.
- The release of internal energy into the motion when colliding atoms end up in a lower internal state or when a molecule is formed.
- The gain of kinetic energy depends on the inelastic channel. On the order of the Zeeman energy, the hyperfine energy, or the molecular vibrational energy. 
- Loss is generally so large that all atoms involved in the collisions are lost.
- Two- or three-body processes.
- Fermionic Feshbach molecular gas 의 경우 bosonic gas와는 다르게 Feshbach resonance 근처에서 안정적이다. Li6 의 경우 10s 정도로 길다. Why? three-body collision 을 하려면 일정 영역에 Fermion 3개가 모여야 되는데, 3개가 모인다면 그 중 2개는 반드시 같은 방향 스핀일 것이므로 3개가 동시에 모이기가 힘들다.)




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

Pethick BEC in dilute gases chapter 5