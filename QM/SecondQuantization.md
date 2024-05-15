다른 표현으로는 Occupation number representation. multi-particle quantum operators 를 명료하게 기술할 수 있다.

N 개의 상태가 있을때, 1번부터 N번까지 각 상태에 존재하는 입자의 갯수 $n_i$ 를 다음과 같이 Fock 상태로 표현한다.

$$
|n_1, n_2,...,n_i,...\rangle
$$

## Indistinguishable particle and Exchange symmetry

구분 불가능한 입자 두개의 상태를 교환해도 관측되는 값은 그대로여야 한다. $|\psi|^2=|(\hat{P}\psi)|^2$ is unchanged. 

이때 exchange operator 에 의한 $\hat{P}\psi$ 는 앞에 phase 가 1이 붙거나 -1 이 붙는 자유도가 있는데(그외의 phase 가 붙는 경우를 anyon 이라고 하는데, 3차원에는 존재하지 않고 2차원에 존재한다), 1이 붙는경우를 Boson, -1이 붙는 경우를 Fermion 이라 한다.

## Creation and annihilation operators

### Boson

$$
a^\dagger_i |n_1, n_2,...,n_i,...\rangle
  = \sqrt{n_i+1}|n_1, n_2,...,n_i+1,...\rangle 
$$

$$
a_i |n_1, n_2,...,n_i,...\rangle
  = \sqrt{n_i}|n_1, n_2,...,n_i-1,...\rangle 
$$

commutation relation

$$
[a_\mu, a_\nu^\dagger] = a_\mu a_\nu^\dagger - a_\nu^\dagger a_\mu = \delta_{\mu\nu}
$$

### Fermion

Fermion 의 경우, 각 상태에 occupation number 는 0 또는 1 뿐이다.

$$
b^\dagger_i |n_1, n_2,...,n_i,...\rangle
  = \begin{cases}
   (-1)^{n_1+n_2+...+n_{i-1}}|n_1, n_2,...,1,...\rangle & \text{if $n_i=0$} \\
  0&  \text{if $n_i=1$}
  \end{cases} 
$$

$$
b_i |n_1, n_2,...,n_i,...\rangle
  = \begin{cases}
  0&  \text{if $n_i=0$}\\
   (-1)^{n_1+n_2+...+n_{i-1}}|n_1, n_2,...,0,...\rangle & \text{if $n_i=1$} \\
  \end{cases} 
$$

Fermion 의 경우, $i$ 번째에 대해서 1번부터 $i-1$ 번까지의 occupation number 에 따라 결정되는 sign 값이 붙는다. 이런 ordering 은 consistency 만 유지한다면 어떤 순서를 잡든 상관없다.

Anti-commutation relation

$$
\{b_\mu, b_\nu^\dagger\} = b_\mu b_\nu^\dagger + b_\nu^\dagger b_\mu = \delta_{\mu\nu}
$$


## Ref

https://phys.libretexts.org/Bookshelves/Quantum_Mechanics/Quantum_Mechanics_III_(Chong)/04%3A_Identical_Particles/4.03%3A_Second_Quantization