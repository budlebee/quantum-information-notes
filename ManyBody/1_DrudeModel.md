Drude model : Ideal gas of electron

Drude model assume that heavy positive unmove particles(similar to nuclear but Drude model was invented before nuclear discovery)

Drude model assume Boltzmann statistics.

Drude model explains conductivity of metals, but cannot explains insulators.

Drude model explains well $Li^+ + e^-$, $Mg^{2+} + 2e^-$, $Cu^+ + e^-$, $Ag^+ + e^-$, $Au^+ + e^-$, but is not good at $Al^{3+}+3e^-$.

Assumtions of Drude model

1. Independent electron approximation. 외부 전기장과 자기장이 없다면, 전자는 충돌과 충돌 사이에 별다른 상호작용 없이 등속 직선운동을 함.

2. 매우 짧은 시간동안 충돌함.

3. 시간 t 와 t+dt 사이 충돌할 확률은 $dt/\tau$. $\tau$는 relaxation time.

4. 전자는 충돌 직후 열평형 상태에 도달한다. 

conductivity of D.C. ($j=\sigma E$)

$$
\sigma = \frac{ne^2 \tau}{m}
$$

very important formula. $n$ 은 number density(단위부피당 전자 갯수), $e$ 는 기본전하, $\tau$는 relaxation time, $m$ 은 전하의 질량 또는 effective mass.

Drude 모델에서 측정한 $\sigma$로 relaxation time $\tau$ 에 이상기체 가정으로 얻은 $v$를 곱하면 mean free path length $v\tau$가 1~10 옹스트롬 정도. 원자 한개정도 크기 이기에 전자가 원자랑 충돌한다고 받아들여졌음(지금 와서는 틀린 픽쳐이지만)

$$
\frac{1}{n}=\frac{4\pi r_s^3}{3}
$$

$$
\frac{dp}{dt} = -\frac{\rho}{\tau}+f(t)
$$

$-\rho/\tau$ 는 충돌로 인한 모멘텀 감소, $f(t)$는 외력에 의한 모멘텀 증감.

## Failure of Drude model

Drude model 로 몇몇 물질들의 classical Hall effect 설명은 가능하지만 classical Hall coefficient 가 음수 나오는 물질들이 있음. Drude model 의 independent electron 가정 fail.

Drude model 의 문제점: number density $n$ 을 너무 100배 정도 크게 산정함. 그리고 전자의 에너지 $mv^2/2$ 를 100배 정도 작게 산정함. 100배와 1/100배가 cancellation 돼서 결과적으로 thermal conductivity 는 관측값과 2,3 배 정도 차이날 뿐 order 는 비슷하게 나오는 것.

Drude model 은 양자역학 이전에 생긴 모델이라서 전자를 이상기체로 다뤄서 볼츠만 분포를 가정하지만,  Fermi Dirac model 로 다뤄야 함. 

### Thermoelectric field

diffusion of charge carrier
$$
E = Q\nabla T
$$

$Q$ is thermo power factor. 이때 charge carrier 가 positive charge 면 Q 는 positive, charge carrier 가 negative 면 Q도 negative.