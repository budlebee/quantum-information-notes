Time-dependent Gross-Pitaevskii equation

$$
i\hbar\frac{\partial}{\partial t}\psi =-\frac{\hbar^2}{2m}\nabla^2\psi +V\psi +U_0|\psi|^2\psi
$$

왼쪽에 $\psi^*$ 를 곱하면,

$$
i\hbar\psi^*\frac{\partial}{\partial t}\psi =-\frac{\hbar^2}{2m}\psi^*\nabla^2\psi +V|\psi|^2 +U_0|\psi|^4
$$

위 방정식의 complex conjugate 는,

$$
-i\hbar\psi\frac{\partial}{\partial t}\psi^* =-\frac{\hbar^2}{2m}\psi\nabla^2\psi^* +V|\psi|^2 +U_0|\psi|^4
$$

원래 방정식에서 complex conjugate 를 빼주면,

$$
i\hbar \left(\psi^*\frac{\partial}{\partial t}\psi + \psi\frac{\partial}{\partial t}\psi^*\right) = -\frac{\hbar^2}{2m}\left( \psi^*\nabla^2\psi + \psi\nabla^2\psi^* \right) 
$$

$$
\frac{\partial}{\partial t}|\psi|^2 + \nabla \frac{\hbar}{2mi}\left( \psi^*\nabla\psi +\psi\nabla\psi^* \right)=0
$$

Continuity equation 

$$
\frac{\partial}{\partial t}n+\nabla (n\bold{v})=0
$$

에 따라, condensate 의 velocity field 를 다음과 같이 정의한다.

$$
v = \frac{\hbar}{2mi} \frac{\psi^*\nabla\psi -\psi\nabla\psi^*}{|\psi|^2} \equiv \frac{\hbar}{m}\nabla \phi
$$

위 정의에 해당하는 Ansatz 는 $\psi = f e^{i\phi}$ 이다. Amplitude f 와 phase $\phi$ 는 real quantity 이고, $f^2=n$ 이다. $\nabla\psi= \nabla (fe^{i\phi})=e^{i\phi} \nabla f +ife^{i\phi}\nabla \phi$, $\nabla\psi^*= \nabla (fe^{-i\phi})=e^{-i\phi} \nabla f -ife^{-i\phi}\nabla \phi$ 이다.

velocity field 가 어느 scalar 함수 $\phi$ 의 gradient 라서, velocity potential 이라고도 부른다.

scalar 함수의 gradient 에 curl 을 취한 것은 0 이므로, 

$$
\frac{\hbar}{m}\nabla \times \nabla\phi = \nabla \times \bold{v} = 0
$$

즉, velocity field 는 irrotational 하다.

또한 velocity field 를 closed loop 를 따라 선적분하면,

$$
\oint \bold{v} d\bold{l} = \frac{\hbar}{m}\oint \nabla\phi d\bold{l} = \frac{\hbar}{m} 2\pi l
$$

$l$ 은 임의의 integer.

## Azimuthal velocity field of a vortex

