## Interaction picture and dyson series

operator in schrodinger picture

$$
H= H_0+V
$$

interaction Hamiltonian

$$
H(t) = H_0 + V(t)
$$

where 

$$
V(t) = e^{iH_0 t/ \hbar}Ve^{-iH_0 t/ \hbar}
$$

state vector in interaction picture is 
$$
|\psi_I(t)\rangle = e^{iH_0t/\hbar}|\psi_S(t)\rangle
$$

time evolution is 

$$
i\hbar\frac{d}{dt}|\psi_I (t)\rangle = V(t)|\psi_I(t)\rangle
$$

Interaction picture 에서의 time evolution 을 $|\psi_I(t)\rangle = U_I(t)|\psi(0)\rangle$ 라고 한다면,

$$
i\hbar\frac{d}{dt}U_I(t) = V(t)U_I(t)
$$

이때 $U_I(0)=1$ 이므로, 양변을 0에서 t 까지 적분하면

$$
i\hbar \left[U_I(t)-U_I(0) \right] = \int_0^t dt' V(t')U_I(t')
$$

$$
U_I(t) =1-\frac{i}{\hbar} \int_0^t dt' V(t')U_I(t')
$$

iteration 을 하면,

$$
U_I(t) = 1 -\frac{i}{\hbar}\int_0^t dt'V(t') + \left(\frac{i}{\hbar}\right)^2 \int_0^t dt'\int_0^{t'}dt''V(t')V(t'')U_I(t'')
$$

보통 first order 까지 쓰고, higher order 를 무한히 계산해 나갈 수 있다.
