# 대칭성(Symmetry)

물리학에서 말하는 대칭성(Symmetry)란, 우리가 관점을 바꾼다 하여도 물리학의 법칙은 바뀌지 않는다는 것이다. 우리가 관찰하는 좌표계의 위치를 바꾸거나 돌린다 해도 자연의 본질은 바뀌어선 안된다(라고 과학자들은 믿고 있고, 그렇게 합의하고 있다).

이런 관점에서의 변환을 대칭 변환(Symmetry transformation)이라고 한다. 대칭 변환은 물리적 상태를 변화시킬수는 있지만, 물리적 법칙은 변하지 않는다. 

양자역학에서 특정 상태 $\Psi$ 가 $\Phi$ 로 전이할 확률(Transition Probability) 는 수학적으로 두 상태 벡터의 내적으로 표현된다. 이때 우리가 다른 관점에서 두 상태를 바라보면 상태 자체는 다르게 보이겠지만, 한 상태에서 다른 상태로 전이하는 물리적 과정은 물리 법칙에 의한 것이기 때문에 전이 확률이 변해선 안된다.

즉 전이 확률이 다음과 같을때, 대칭 변환은 전이 확률 $P(\Psi\rightarrow\Phi)$ 를 보존시키는 모습을 가져야 할 것이다.
$$
P(\Psi\rightarrow\Phi) = |\braket{\Phi|\Psi}|^2
$$

대칭변환을 연산자(Operator) $U$ 라고 하자. $\Psi$와 $\Phi$를 $U$로 변환하면 다음과 같다.

$$
P(\Psi\rightarrow\Phi) = |\braket{U\Phi|U\Psi}|^2
\\
=|\braket{\Phi|U^{\dagger}U|\Psi}|^2=|\braket{\Phi|\Psi}|^2
$$

따라서 대칭변환은 $U^{\dagger}U=I$ 이고, $U^{\dagger}=U^{-1}$을 만족해야 함을 알 수 있다. 이와 같은 성질의 연산자를 유니터리(Unitary) 연산자라고 한다.

그럼 몇가지 가정을 해보자. 아주 작은(infinitesimal) $\epsilon$ 만큼 상태를 변화시키는 유니터리 연산자를 $U=I + i\epsilon T$ 라고 쓰는 것이다. 그럼 유니터리 조건에 따라서, 

$$
U^{\dagger}U=(I-i\epsilon T^{\dagger})(I+i\epsilon T)=I-i\epsilon T^{\dagger}+i\epsilon T+i\epsilon^2 T^{\dagger}T=I
$$

이어야만 한다. 우리가 만들고자 하는 양자역학 시스템이 Linear 하다고 가정한다면, infinitesimal $\epsilon $의 제곱인 항을 무시할 수 있고, 그렇다면 $T^{\dagger}=T$ 임을 알 수 있다.

무한히 큰 $N$ 에 대하여 $\epsilon=\theta/N$ 라고도 쓸수 있을 것이다. $\epsilon$ 만큼의 변환을 $N$ 번 한것이 $\theta$만큼의 변환이라고 생각한다면, 다음과 같이 주장할 수 있다.
$$
[I+i\theta T/N]^N = \sum_{k=0}^{N}{N \choose k}(\frac{i\theta T}{N})^k
$$

CLAIM : 이때 $N$ 이 충분히 크다면, ${N \choose k}\frac{1}{N^{k}} \approx \frac{1}{k!}$ 으로 쓸 수 있을 것이고, 그럼 위 식의 우변은 $e^{i\theta T}$의 테일러 전개(taylor expansion) 형태가 된다.

$$
[I+i\theta T/N]^N \rightarrow e^{i\theta T} = U(\theta)
$$

 $T$가 허미시안(Hermitian) 연산자이기 때문에, $e^{i\theta T}$를 테일러 전개한 것에 아이젠벡터를 작용하면 모든 $T$ 가 해당하는 어떤 아이젠밸류 $\alpha$로 대체될 것이고, 해당 아이젠밸류에 대한 테일러 전개를 다시 표현하면 $e^{i\theta \alpha}$가 된다. $e^{i\theta \alpha}$ 의 절댓값 크기는 1이므로, 대칭 연산자를 exp 함수의 꼴로 표현해도 norm 이 보존된다는 것을 확인할 수 있다.

## ref

Steven Weinberg, Lecture on Quantum Mechanics