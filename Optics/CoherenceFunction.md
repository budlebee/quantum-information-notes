# Coherence (결맞음)

일반적으로 말하는 결맞음(coherence)는 빛의 1차 간섭성으로, 2중 슬릿 실험 등에서 빛이 얼마나 간섭무늬를 형성할 수 있는지에 대한 것이다. 즉, 빛의 위상이 규칙성을 유지하는지 못하는지에 대한 것이다.

coherence 는 1차, 2차, ... n차 coherence 가 있는데, 2차 coherence 는 빛의 응집성(bunching 과 anti-bunching)과 관련된 특성이다.

## 1st-order coherence

### coherence time

보통 빛의 위상상태를 정확히 예측할 수 있는 빛을 coherent light 라고 한다. 단색광(monochromatic light)는 $E(t) = E_{0}\sin{ωt}$로 표현할 수 있고, 아무리 긴 시간 뒤에도 빛의 위상을 정확히 예측할 수 있다.

하지만 무한히 coherence 를 유지할 수 있는 빛은 unphysical 하고, 위상을 유지하는데 어느 정도 유한한 한계를 갖게 된다. coherence 를 유지할 수 있는 시간을 coherence time 이라고 하고, coherence time 에 빛의 진행속도 c 를 곱한 것을 coherence lenght, 결맞음 길이라고 한다.

영의 이중슬릿 실험이나 마이컬슨 몰리 간섭계 같은 실험의 경우, 두 빛의 경로차가 결맞음 길이보다 짧아야지 간섭 무늬를 얻을 수 있다.

이상적인 경우 들뜬 상태의 원자에서 방출되는 빛은 sine wave 이겠지만, 원자가 다른 원자와 충돌하면서 상호작용을 일으키고 에너지 준위에 변화가 생긴다. 이로 인해 방출되는 빛의 형태도 변하게 된다. 충돌이 멈추면 다시 sine wave 가 방출되겠지만, 이때 나오는 sine wave 는 앞서 나온 sine wave 와는 다른 시점을 가진(다른 위상을 가진) 빛이 된다. 

또한 원자의 움직임으로 인한 도플러 효과로 인해 빛의 주파수가 변하게 된다. 이러한 효과들로 인한 주파수의 변화와 결맞음 시간을 수식으로 표현하면 다음과 같은 관계가 있다. $\Delta w = 1/\tau_C$. 즉, 주파수 bandwidth 에 큰 변화가 생기는 경우 결맞음 시간은 짧다.

### 결맞음의 양자이론

전기장을 소멸연산자와 생성연산자로 쓰면

$$
E(r,t) = i\sum_{k} \epsilon_{k}\sqrt{\frac{\hbar w}{2\epsilon_{0}V}}(\hat{a}_{k}e^{i(k\cdot r-w_{k}t)} - \hat{a}_{k}^{\dagger}e^{-i(k\cdot r-w_{k}t)}) = E^{+}(r,t) + E^{-}(r,t)
$$

빛을 관측하는 행위는 빛을 흡수하는 과정이니 소멸연산자를 포함하는 $E^{+}(r,t)$ 부분이 빛의 관측과 관련된 부분이다. 따라서 빛이 상태 \ket{i} 에 있을때 시각 t에서 r 에 위치한 검출기에서 빛을 관측할 확률 P 는 $\sum_{f} |\bra{f}E^+ \ket{i}|^2$ 에 비례한다.

$$
P \propto \sum_{f} |\bra{f}E^+ \ket{i}|^2 = \sum_{f} \bra{i}E^{-} \ket{f}\bra{f}E^{+} \ket{i} = \bra{i}E^- E^+ \ket{i} =Tr[E^- E^+ \rho]
$$

by completeness relation $\sum_{f} \ket{f}\bra{f} = I$

