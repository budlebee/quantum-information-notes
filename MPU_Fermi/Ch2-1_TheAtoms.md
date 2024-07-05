Window for degenerated Fermi gas: $10^{11}/cm^3<n < 10^{15}/cm^3$. 밀도가 너무 낮다면 thermalization 이 느리고, 밀도가 너무 높다면 3-body collision 으로 인한 로스가 높아짐.

밀도가 $10^{14}/cm^3$ 정도 되는 BEC 의 경우 3-body 로스가 주요 로스이지만, 페르미 가스의 경우 Pauli principle 로 인해 작은 공간에 3개의 Fermion 이 모이는 경우가 줄어들어서 3-body 로스가 작아짐. 반면, molecluar state 의 사이즈가 Fermi wavelength 정도가 된다면 3-body relaxation 이 억제되지 않음 (자세한 것은 섹션 2.4.2)

Feshbach 레조넌스로 상호작용 세기를 조절할 수 있다는 장점. BCS 사이드의 경우, weak interaction 때문에 critical temperature 가 기하급수적으로 낮음. 그래서 BCS 영역을 보려면 degenerated temperature 보다 훨씬 더 냉각해야함.

## Atoms

안정된 Fermion 동위원소는 많지 않음. 주로 6Li 와 40K 에 대해 다룰 것.

6Li의 경우 $m_s=-1/2$ 인 상태중에 low field seeking state 가 없음. 자기장 트랩에 잡히는 상태들은 전부 high field seeking 이라서, spin relaxation 이 있을 수 있음.

40K의 경우 $m_s=-1/2$ 인 상태 중 하나가 low field seeking 임.

hyperfine structure 들의 자기장에 대한 기울기는 자기장이 클때 대략 1.4MHz/G. 자기장이 크면 Zeeman splitting 이 우세하므로, $H_{hf}\simeq g_s \mu_B B\cdot S$ 로, $g_s\simeq 2$, $\mu_B\simeq$ 2.8MHz/G 정도라서 그렇다.

## Collision

보통 van der Waals potential 로 인한 range 가 $r_0\simeq (mC_6/\hbar^2)^{1/4}$ 정도고, $r_0$ 가 thermal de Broglie wavelength $\lambda_T$ 보다 작다면 원자들은 서로 상호작용 없이 "fly by" 하게 된다. 

Pauli 원리에 의해 같은 상태의 Fermion 끼리는 s-wave scattering 을 안한다. p-wave scattering 이 억제되는 6Li 온도는 대략 6mK 정도인데, quantum degeneracy 가 되는 온도보다는 높으므로, 리튬 원자를 더 냉각하고 싶다면 다른 원자나 다른 하이퍼파인 상태를 이용한 thermalization 과 evaporation 이 필요하다.

### Inelastic collision

* Spin relaxation: 보통 inelastic collision 으로 인한 spin relaxation rate 는 $10^{-11}cm^3/s$ 정도로, 앞서 설명한 $10^{11}/cm^3$~$10^{15}/cm^3$ 의 밀도에서는 ms 정도의 타임스케일로 빠르게 decay 한다고 볼 수 있다. 스핀 릴렉세이션은 스핀 교환시 더 낮은 내부 에너지 상태가 존재할때만 발생하므로, 그런 상태가 존재하지 않는 mixture 의 조합에서는 spin relaxation 이 억제된다 (Na-Li 의 동조냉각에서 stretched state 를 이용하는 것).

* Dipolar relaxation: 전자 또는 핵의 각운동량이 원자의 상대적인 움직임으로 전이되는 것. $10^{-15}cm^3/s$ 정도로 천천히 진행된다. BEC의 경우 마그네틱 트랩에 잡혀있을때 dipolar relaxation 에 의해 스핀이 돌아가면서 로스가 생길 수 있다.

* Feshbach resonance: FB 근처에서는 모든 inelastic proceeses 들이 강하게 일어난다. 

두개의 가장 낮은 hyperfine 상태의 리튬을 optical trap 으로 붙잡는 경우, 로스 메커니즘은 dipolar relaxation 인데, FB resonance 근처에서도 dipolar relaxation 로스가 작다. 그 이유를 추측하기로는 리튬의 경우 하이퍼파인 에너지가 작고, 질량이 작고 van der Waals coefficient $C_6$가 작아서 d-wave exit channel에 대한 centrifugal barrier 가 높기 때문이라고 한다 (?).

by THkim: centrifugal potential 의 경우 

$$
\hat{V}=V+\frac{\hbar^2}{2\mu}\frac{l(l+1)}{r^2}
$$

이때 selection rule 에 의해서 $\triangle L =0,2$ 인데 dipolar relaxation 은 motional angular momentum 에 의한 것, 즉 $\triangle L =2$ 인 경우(d-wave). 이때 van der Waals 반지름이  $r_0\simeq (mC_6/\hbar^2)^{1/4}$ 라서 작고, centrifugal potential 에서 $r$이 작으니 centrifugal barrier 가 크다고 말하는 것.

Na-Li 의 경우 커다란 DFG 를 만드는데 좋은 특성들을 갖고 있다고 한다.

