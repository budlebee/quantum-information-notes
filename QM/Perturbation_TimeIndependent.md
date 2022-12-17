# Non degenerate time independent perturbation

Yayleigh-Schrodinger perturbation theory 라고도 불리는 방법.

전체 해밀토니안 $H$ 에서 우리가 해석적으로 풀수 있는 해밀토니안을 $H_0$ 라고 하고, 그렇게 풀 수 없는 해밀토니안 부분을 $V$ 라고 하면, $H=H_0+V$ 이다.

$H_0$ 의 eigenstates 를 $\ket{n^{(0)}}$ 이라고 하고, eigenvalues 를 $E_n^{(0)}$ 라고 하자.

$H_0\ket{n^{(0)}} = E_n^{(0)}\ket{n^{(0)}}$ 일때, $H\ket{n} = E_n\ket{n}$ 인 $\ket{n}$ 과 $E_n$ 을 찾는 것이 목표다.

perturbation 은 외부에서 걸어주는 전기장이나 자기장 같은 것이 될테고, 이런 퍼터베이션을 조절할 수 있는 파라미터를 $\lambda$ 라고 하자.

$$
H\ket{n} = (H_0+\lambda V)\ket{n} = E_n\ket{n}
$$

라고 쓸 수 있고, $\lambda =0$ 이면 unperturbed, $\lambda =1$ 이면 fully perturbed 상황이다.
$$
E_n - E_n^{(0)}\equiv \triangle_n
$$
이라고 energy shift 를 정의하면,

$$
(E_n^{(0)}-(H_0+\lambda V)+\lambda V)\ket{n} = (E^{(0)}_n - E_n +\lambda V)\ket{n} = (\lambda V - \triangle_n)\ket{n}
$$

이 된다.

이때 $H_0$ 는 Hermitian operator 이므로 왼쪽 bra 에 작용해도 똑같다는 성질을 이용하면,

$$\bra{n^{(0)}}(\lambda V - \triangle_n)\ket{n} = \bra{n^{(0)}}(\lambda V - E_n+E_n^{(0)})\ket{n}\\
 = \bra{n^{(0)}}(E_n^{(0)}-H_0)\ket{n}=0 $$

 따라서 $(\lambda V - \triangle_n)\ket{n}$ ket 은 $\ket{n^{(0)}}$ 성분이 없다.

complementary projection operator 를 다음과 같이 정의하자.

$$
\phi_n \equiv 1-\ket{n^{(0)}}\bra{n^{(0)}} = \sum_{k\neq n}\ket{k^{(0)}}\bra{k^{(0)}}
$$

$(E_n^{(0)}-H_0)$ 의 inverse operator 를 $1/(E_n^{(0)}-H_0)$ 라고 쓰자. 

...

결과적으로, 

$$
\triangle = E_n - E_n^{(0)} = \lambda V_{nn} +\lambda^2 \sum_{k\neq n}\frac{|V_{nk}|^2}{E_{n}^{(0)}-E_k^{(0)}} + ...
$$
where $V_{nk}\equiv \bra{n^{(0)}}V\ket{k^{(0)}}\neq \bra{n}V\ket{k}$, unperturbed matrix elements.

그리고 perturbed ket 은

$$
\ket{n}=\ket{n^{(0)}} + \lambda \sum_{k\neq n}\ket{k^{(0)}}\frac{V_{kn}}{E_n^{(0)}-E_k^{(0)}}\\
+\lambda^2(\sum_{k\neq n} \sum_{l\neq n}\frac{\ket{k^{(0)}}V_{kl}V_{ln}}{ (E_n^{(0)}-E_k^{(0)})(E_n^{(0)}-E_l^{(0)}) }-\sum_{k\neq n}\frac{\ket{k^{(0)}}V_{nn}V_{kn}}{(E_n^{(0)}-E_k^{(0)})^2})+...
$$


# Degenerate time independent perturbation

perturbation 이 없을 때 degeneracy 가 있는 경우, $\frac{V_{kn}}{E_n^{(0)}-E_k^{(0)}}$ term 의 denominator 가 0 이 돼서 위의 공식들을 쓸 수 없다.

해결법 : $V_{nk}=0$ 이고 $n\neq k$ 인 basis 를 찾는다.

g-fold degeneracy 가 있는 경우, degeneracy 가 있는 subspace 를 D 라고 하자. 그리고 해당 degeneracy 의 energy 를 $E_D^{(0)}$ 라고 하고, eigenstates 를 ${\ket{m^{(0)}}}$ 라고 하자.

일반적으로 perturbation 이 생기면 degeneracy 가 없어지고 전부 구분 가능한 상태가 되므로, 그때의 상태를 $\ket{l}$ 이라고 하자. 이때 perturbation 의 정도 $\lambda$ 를 0으로 보내면, $\ket{l}\rightarrow \ket{l^{(0)}}$ 이 될 것이다. 

$\ket{m^{(0)}}$과 $\ket{l^{(0)}}$ 둘다 같은 subspace 를 span 하고 eigenvalue 도 같지만, 둘이 같은 상태는 아니라고 하자 (마치 H/V basis 와 D/A basis 처럼). 그럼 basis change 에 의해

$$
\ket{l^{(0)}} = \sum_{m \in D}\braket{m^{(0)}|l^{(0)}}\ket{m^{(0)}}
$$

$
H\ket{l}= E_l\ket{l} = (H_0 +\lambda V)\ket{l}
$ 에 대해, $\triangle_l \equiv E_l -E_D^{(0)}$ 라고 하면,

$$
(E_D^{(0)}-H_0)\ket{l} = (\lambda V - \triangle_l)\ket{l}
$$

이 된다. $\ket{l} = \ket{l^{(0)}}+\lambda \ket{l^{(1)}}+...$, $\triangle_l = \lambda \triangle_l^{(1)}+\lambda^2 \triangle_l^{(2)}...$, 로 확장하면, $\lambda$ first order 에 대해서
$$
(E_D^{(0)}-H_0)\ket{l^{(1)}} = (V-\triangle_l^{(1)})\ket{l^{(0)}}\ket{l^{(0)}}= (V-\triangle_l^{(1)})[\sum_{m \in D}\ket{m^{(0)}}\braket{m^{(0)}|l^{(0)}}]
$$

왼쪽에 $\bra{m'^{(0)}}$를 작용하면, $\bra{m'^{(0)}}(E_D^{(0)}-H_0)=0$ 이므로
$$
\sum_{m\in D}\bra{m'^{(0)}}V\ket{m^{(0)}}\braket{m^{(0)}|l^{(0)}}\\
=\sum_{m\in D}V_{m'm}\braket{m^{(0)}|l^{(0)}}
=\triangle_l^{(1)}\braket{m'^{(0)}|l^{(0)}}
$$

eigenvalue 를 구하면 1st order energy shift 를 구할 수 있다.

$\ket{m^{(0)}}$ 의 공간으로 proejction 하는 projector 를 $P_0=\sum_{m\in D} \ket{m}\bra{m}$ 라고 하고, 그외의 공간으로 proejction 하는 것을 $P_1=1-P_0$ 라고 하자. 그러면

$$
0 = (E-H_0-\lambda V)\ket{l} = (E-H_0 -\lambda V)P_0\ket{l} +(E-H_0 -\lambda V)P_1\ket{l} \\
= (E-E_D^{(0)} -\lambda V)P_0\ket{l} +(E-H_0 -\lambda V)P_1\ket{l} 
$$

로 쓸 수 있고, 위 식에 $P_0$ 프로젝터를 가했을때와 $P_1$ 를 가했을때를 적으면, 정의에 따라 $P_0P_0=P_0$, $P_0P_1=0$ 이므로

$$
(E-E_D^{(0)} -\lambda P_0V)P_0\ket{l} - \lambda P_0 V P_1\ket{l}
$$

$$
- \lambda P_1 V P_0\ket{l} + (E-E_D^{(0)} -\lambda P_1V)P_1\ket{l} 
$$

이때 $P_1$ 에 대한 subspace 는 singular 문제에서 자유로워 지므로, 