# Linear response theory

So many observables are approximately linear

- Susceptibility $P=\chi E$
- Dielectric function $D=\epsilon E$
- Conductivity $J=\sigma E$
- Magnetic susceptibility $M=\chi_m H$

and so on.

Induced quantity by external field can be represented as 

$$
\frac{\vec{m}(w)}{V} = \tilde{\chi}(w)\vec{F}(w)
$$

where 

- $\vec{m}$ : induced response (ex: current)
- $V$ : volume of the system
- $\vec{F}$: applied external field

# Kubo formula

formula for general susceptibilites $\tilde{\chi}(w)$

(tilde means Fourier transformed-components)

$$
\frac{\vec{m}(w)}{V}=\tilde{\chi}(w)\vec{F}(w)
$$

$$
\tilde{\chi}_{\mu\nu}(w)=\frac{i}{\hbar V}\int_{0}^{\infty}d\tau e^{(i\omega -\eta)\tau}\braket{[\tilde{M}_{\mu}(\tau),\tilde{M}_{\nu}(0)]}_0
$$


## removing q-dependency in conductivity

In solid, lattice interval ~ 1A.

optical range $\lambda$ ~ 1nm to 1mm.

In k-space, for optical wavelength, $q=\frac{2\pi}{\lambda}<<\frac{2\pi}{a}$, we can neglect q.

but out of optical range(ex. X-ray), we cannot neglect q-dependency.