
## Two level transition

* Ultracold 상황에서는 s-wave 를 제외한 higher order scattering 이 억제됨. 

* Fermion 의 파동함수는 anti-symmetric 이므로, 같은 종류의 입자로만 이루어져 있다면(spin 파동함수가 symmetric 하다면) symmetric 한 s-wave scattering 은 잘 일어나지 않음. 그래서 two-component mixture 를 사용하는 것.

* two-component mixture 를 만드는 법

1. MOT 다음단계에서 optical pumping

2. pure single-component gas 에서 RF 를 쏴주는 것.

* RF 는 3m 가량의 매우 긴 파장을 갖고 있고, momentum kicking 이 무시될 수 있을만큼 작다.

* 보통 RF 안테나는 수 센티미터 정도이고 샘플의 크기는 수백 마이크로 미터 정도이기 때문에, 샘플에 가해지는 RF 빔은 constant 하다고 볼 수 있다.

* RWA 를 통한 two level system 해밀토니안으로 기술할 수 있음.

### Rabi oscillation 을 이용한 transition

Rabi frequency $\omega_R/2\pi$ 는 대략 수 kHz.  


### Landau-Zener field sweep 을 이용한 transition

RF 필드의 detuning 을 $\delta$ 라고 할때, $\delta \gg \omega_R$ 인 영역에서 부터 $-\delta$ 까지 sweep.

$$
P_{1\rightarrow 2} = 1-\exp(-2\pi \omega_R^2/\dot{\delta})
$$

RF pulse 를 쓰든 field sweep 을 쓰든 샘플은 여전히  coherent 를 유지한 채 fully polarized superposition state of 1 and 2.

## Clock shift

원자끼리의 상호작용으로 인한 density dependent shift. 이름의 유래는 atomic fountain clock 의 리밋을 결정해서 clock shift 라고 한다. mean-field shift, collisional shift 등으로도 불린다.

virtual scattering process 로, $U_0^2$ 에 비례하는 실제 스캐터링 과정과는 다르게 $U_0$ 에 비례한다.

two-state Fermi mixture 에서는 clock shift 가 없다고 하는데(why?), three-component 에서는 있다고 한다.

만약 상태 1과 2가 incoherent 하게 섞여 있다면 $|2\rangle$ 의 원자들은 $|1\rangle$ 원자들이 만들어 내는 mean field 를 느낄 것. 그래서 에너지 shift 는 $\delta E_2 = 4\pi\hbar^2a_{12}n_1/m$, 이때 $a_{12}$는 두 상태의 scattering length 이고 $n_1$ 은 1번 상태의 밀도이다. 

하지만 RF pulse 를 이용한 transition 은 coherent 하게 $|1\rangle$ 상태를 $\cos{\alpha}|1\rangle + e^{i\phi}\sin{\alpha}|2\rangle$ 로 전환하는 것. 그래서 clock shift 를 느끼지 않는다. RF spectroscopy 실험에서도 two-component Fermi gas 에서는 clock shift 가 없음이 보여졌다. 

RF 로 인한 rotation 은 energy hamiltonian 과 commute 하다. 그래서 no shift.

### Absence of clock shift in incoherent two-component Fermi mixture

하지만 incoherent 한 two-component Fermi mixture 에서도 clock shift 가 없다(ref: Spectroscopic Insensitivity to Cold Collisions in a Two-State Mixture of Fermions, 2003). 

many-body 시스템에서 상호작용 에너지는 coherent collision(들어오는 두 입자의 상태와 나가는 두 입자의 상태가 같은 것)으로 결정된다. 그럼 이 경우 두 입자는 (1)각자의 운동량을 보존하거나, 아니면 (2)서로의 운동량을 교환하거나 두가지 뿐이다.

-> 관련 레퍼런스 읽어보았지만 아직도 왜 RF 가 coherence 를 re-introduce 하는지 납득이 안됨. 

### RF 실험에서 6Li의 특별함

6Li는 hyperfine interaction 이 작아서 수백 가우스 정도면 nuclear spin 과 electron spin 을 decouple 할 수 있다. 또한 nuclear spin 만 뒤집는 transition 이 weak field sensitivity 를 갖고 있다.

예를 들면, 600G 이상에서 1-2 resonance 의 field dependence 는 2.7kHz/G 보다 작다. 그에 반면 40K 같은 경우 202G Feshbach resonance 근처에서 2-3 transition 의 field dependence 는 170kHz/G 나 된다.


## Decoherence

* RF 는 decoherence 를 만들지 않음

* 원자가 불균일한 trap 을 지나면 각기 다른 phase 를 갖게 됨. 

* incoherent mixture 가 된다면 더이상 같은 quantum state 가 아니게 되므로, 원자들끼리 s-wave scattering 을 할 수 있게 됨.

* decoherence time scale 은 대략 수십 ms.