

# Sensing

기존 간섭계 센싱 : laser 가 강할 수록 크기를 키워서 더 높은 해상도를 얻을 수 있지만, laser 가 세지면 radiation pressure 가 간섭계 거울등을 흔들어서 안정성이 떨어지게 됨.

Carlton M. Caves : 그럼 quantum light 를 쓰는건 어떨까?

크게 두 종류의 센싱 : Atom-based quantum sensing, Heisenberg quantum sensing

### 1. Atom-based quantum sensing 

classical stmulus (laser, or) -> (atom <-> analyte) -> classical response

주로 sensitivity 를 중시

### 2. Heisenberg quantum sensing

quantum state light -> analyte -> quantum state light

얽힘이나 압축 등을 활용. quantum state light 의 변화를 보는 것.

주로 precision 을 중시

Mean Square Error 

$$
MSE(x) = \braket{(x_{est}-x_{true})^2}=\braket{(x_{est}-\braket{x_{est}})^2} + (\braket{x_{est}}- x_{true})^2
$$

여기서 첫번째 텀이 precision 이고, 두번째 텀이 accuracy 임.

실험실 상황에서라면 $x_{true}$ 를 이미 알고 있으니 accuracy 는 튜닝이 가능함. 

## Quantum sensing bound

shot noise 와 연관 (buncing, anti-bunching property 가 중요할까?)

quantum sensing 은 크게 4가지 단계.

1. 상태 준비
2. 상태 인코딩
3. measurement
4. detection

1,3,4 를 최적화 했다면 Quantum Cramer-Rao error Bound (QCRB) 가 센싱 에러의 바운드가 됨.

## Issues of quantum sensing

- Optimal state preperation 
- Optimal measurement
- loss and decoherence

QCBR 은 $1/\triangle n$ 에 비례. 그럼 $\triangle n$ 이 무한대로 가면, 페이즈 센싱 에러를 0으로 줄일 수 있을까?

예를 들면, Riemann-Zeta 나 beta-negative, Yule-Simon distribution 처럼 heavy tale distribution 으로 불리는 것들은 $\braket{(\triangle n)^2}$ 이 무한대임 (실제로 양자 상태가 저런 통계적 분포를 가지게 할 수 있는지는 차치하고).

Sensing 에서 얻어내는 정보를 정량화 하는 것은 prior information 이 중요. 요즘(2022)은 베이지안 관점으로 이론적 연구함. Fisher information 이나 QCBR 만 보면 misleading 할 수 있으니 주의.

## Ghost imaging

IR 영역대는 디텍션 효율이 낮으니, non-degenerate spdc 를 이용해서 IR 영역 정보를 얻고, 측정은 non-IR 영역대(효율이 좋은곳)을 측정하는 식으로 imaging 이득 얻기.