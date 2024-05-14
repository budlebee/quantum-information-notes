
# Spantaneous Parametric Down Conversion (SPDC)

Spontaneous parametric down-conversion (SPDC) is a nonlinear optical process mediated by the $\chi^{(2)}$ anisotropic medium. Incident pump photon inside $\chi^{(2)}$ medium interact with quantum vacuum to down-convert into signal-idler photon pair. \par 
To describe SPDC, there are some assumptions.\par
* Medium is non-magnetic. $\vec{M}=0$ and $\vec{B}=\mu_0 \vec{H}$.
	
* Medium is approximately lossless. interacting light frequency spectrum is far enough from any absorption bands. 
	
* Pump light is weak compared to the electric field of binding electrons to their atoms. The induced polarization field $\vec{P}$ is expressed as a rapidly decaying power series in applied electric field $\vec{E}$:
$$
			P_i = \varepsilon_0[\chi_{ij}^{(1)}E_j+\chi_{ijk}^{(2)}E_j E_k+\chi_{ijkl}^{(3)}E_j E_k E_l+...]
$$
where $\chi$ is susceptibility tensor.



Energy density $u$ of optical field in a medium is 

$$
		u = \frac{1}{2} (\vec{E}\cdot\vec{D}+\vec{B}\cdot\vec{H})
$$

Displacement field $\vec{D}$ is $\vec{D}=\varepsilon_0\vec{E}+\vec{P}$, so interaction Hamiltonian related to second order induced polarization and external pump field is

$$
	H_{SPDC} = \frac{\varepsilon_0}{2}\int dV \chi^{(2)}E_p E_s E_i
$$
Subscript $p$ denotes pump field, and $s$ and $i$ denote signal and idler, which are the results of SPDC process.

For simplicity, we assume continuous-wave laser pumping. We treat pump laser field as classical field and induced fields as quantum fields. The interaction Hamiltonian becomes

$$
		H_{SPDC} = \frac{\varepsilon_0}{2}\int dV \chi^{(2)} E_p \hat{E}_s^{(-)} \hat{E}_i^{(-)}\\ \nonumber
		=\frac{\varepsilon_0 A}{2}\int_{-L/2}^{L/2} dz \chi^{(2)} E_p \hat{E}_s^{(-)} \hat{E}_i^{(-)}
	$$
where
$$
		\hat{E}^{(-)} = \frac{1}{\sqrt{2\pi}} \int dw \sqrt{\frac{2\hbar w}{c \varepsilon_0 A}} \hat{a}^{\dagger}(w) e^{-i(k(w)z-wt)}	
$$
$A$ is interaction area with medium and pump field. $L$ is length of medium.

We can expand interaction Hamiltonian as follows

$$
		H_{SPDC} =\frac{\hbar }{2\pi c}\int_{-L/2}^{L/2} dz \int dw_s \int dw_i \chi^{(2)} E_p \sqrt{w_s w_i} \\ 
		\times e^{-i(k_p -k_s(w_s)-k_i(w_i))z} e^{-i(w_p -w_s-w_i)t} \hat{a}^{\dagger}_s (w_s) \hat{a}^{\dagger}_i (w_i)
$$
Let define $\triangle k \equiv k_p-k_s(w_s)-k_i(w_i)$. Following integral shows the \textit{phase matching} condition of SPDC.
$$
		\int_{-L/2}^{L/2} dz e^{i\triangle k z}=Lsinc\left(\frac{\triangle k L}{2}\right)
$$
When $\triangle k=0$, value of sinc function is maximum and probability of SPDC is maximum. The amplitude decreases rapidly out of phase matching $\triangle k \neq 0$.

With this phase matching condition, interaction Hamiltonian can be written as
$$
	H_{SPDC} = \frac{\hbar E_p L }{2\pi c}\int dw_s \int dw_i \chi^{(2)} \sqrt{w_s w_i} sinc\left( \frac{\triangle k L}{2} \right) e^{-i(w_p-w_s-w_i)t} \hat{a}^{\dagger}_s (w_s) \hat{a}^{\dagger}_i (w_i)
$$
Initial state is vacuum state $|0\rangle$ and first order perturbation by this interaction Hamiltonian is 

$$
	\hat{U} = \exp{\left( -\frac{i}{\hbar}\int dt H_{SPDC} \right)} \simeq 1-\frac{i}{\hbar}\int dt H_{SPDC}
$$
$$
		|\psi\rangle = -\frac{i}{\hbar}\int_{-\infty}^{\infty} dt H_{SPDC}
$$
By the following delta function formula, we can derive energy conservation condition of SPDC.

$$
	\int_{-\infty}^{\infty}dt e^{i(w-w')t}=2\pi \delta (w-w')
$$
$$
		|\psi\rangle = C\int dw_s \int dw_i \sqrt{w_s w_i} sinc\left(\frac{\triangle k L}{2}\right) \delta(w_p-w_s-w_i)\hat{a}^{\dagger}_s (w_s) \hat{a}^{\dagger}_i (w_i) |0\rangle
$$
$C$ is constant containing all constants from the previous derivation. Delta function $\delta(w_p-w_s-w_i)$ shows the energy conservation $w_p=w_s+w_i$.

From this SPDC wave function Eq. \ref{eq_spdc}, we know that SPDC process generates photon pair.

Polarization plays an important role in the SPDC process. Phase matching is closely related to the refractive index, crystal class, permutation symmetries \cite{boydBook, sellmeier,bbo}. SPDC crystals can be classified in three types:

* Type-0 : polarization of pump, signal, idler photons are same.
* Type-1 : signal and idler photons have same polarization but pump photon is orthogonal.
* Type-2 : signal and idler photons have perpendicular polarization.
\end{itemize}

In this thesis, we mainly utilize type-2 SPDC process that pump field is horizontal and signal/idler pair is horizontal/vertical polarization.

With the consideration of multi-pair generation in SPDC, the wave function of SPDC can be written as follows
$$
		|\psi_{type-2}\rangle = \sqrt{1-p^2}\sum_{n=0}^{\infty} p^n |n\rangle_H |n\rangle_V

$$
where $p$ is the probability that SPDC takes place and $n$ denote photon-number state. Subscripts $H$ and $V$ denote polarization of generated photon.

--- below is old version ---

pump photons inside a $\chi^{(2)}$ nonlinear medium interact with quantum vacuum to down-convert into signal-idler photon pairs.

Spontaneous : because there is initially no field at the signal or idler frequencies.

optical parametric processes are equated involing no net excahnge of energy or momentum with the nonlinear medium. Thus, we can treat SPDC as the quantum evolution of a closed system.

## Three assumptions of SPDC

1. Material is non-magnetic, so that $\vec{M}=0$ and $\vec{B}=\mu_0 \vec{H}$

2. Material is approximately lossless. interacting light frequency spectrum is far enough from any absorption bands. 

3. Pump light is weak compared to the electric field of biding electrons to their atoms. The polarization field $\vec{P}$ is expressed as a rapidly decaying power series in applied electric field $\vec{E}$:

$$
P_i = \epsilon_0[\chi_{ij}^{(1)}E_j+\chi_{ijk}^{(2)}E_j E_k+\chi_{ijkl}^{(3)}E_j E_k E_l+...]
$$

$\chi^{(n)}$ is $n$ th order optical suscepibility tensor. Most crystalline materials respond differently to fields polarized along its different principal axes, the induced polarization will not always same direction as the applied electric field. 

## Nonlinear Hamiltonian

energy density of an optical field in a medium is 

$$
U = \frac{1}{2}\int d^3r(\vec{E}\cdot \vec{D}+\vec{B}\cdot\vec{H})
$$

and $\vec{D} = \epsilon\vec{E} = \epsilon_0\vec{E}+\vec{P}$. Thus, 
$$
H^{(2)}_{NL}=\frac{\epsilon_0}{2}\int d^3r \chi^{(2)}_{ijk}E_i E_j E_k
$$

Electric field is written as a linear combination of bosonic ladder operators is inconsistent with the Maxwell equation in the nonlinear regime and leads to incorrect expressions for three or higher-order nonlinear processes.

Thus we convert electric field $\vec{E}$ into a displacement field $\vec{D}$, as

$$
E_i = \zeta^{(1)}_{ij}D_j+\zeta^{(2)}_{ijk}D_j D_k +\zeta^{(3)}_{ijkl}D_j D_k D_l + ...
$$

where $\zeta$ is inverse optical susceptiblity tensor.

Finally, nonlinear Hamiltonian is

$$
H^{(2)}_{NL} = \int d^3r \zeta^{(2)}_{ijl}(r)D_i(r) D_j(r) D_l(r)
$$

### Field quantization

$$
D = D^{(+)}+D^{(-)}
$$
$$
\hat{D}^+ = \sum_{s,\vec{k}} i\sqrt{\frac{\epsilon_0 n^2(\vec{k})\hbar w(\vec{k})}{2V}}\hat{a}_{s,\vec{k}}(t)\hat{\epsilon}_{s,\vec{k}}e^{i\vec{k}\cdot\vec{r}}
$$

And $\hat{D}^-$ is the Hermitian conjugate of $\hat{D}^+$. $\vec{k}$ is the momentum of photon and $\vec{\epsilon}_{s,\vec{k}}$ is the polarization vector with polarization index $s$. V is the quantization volume which we may take to approach infinity in the continuum limit.

Nonlinear Hamiltonian has eight distant terms. Various combinations of these terms correspond to diffrent basic nonlinear optical processes. But for many non-linear medium, $\zeta^{(2)}$(or $\chi^{(2)}$) is only significant for one particular optical process by material design

(Even $\zeta^{(2)}$ is significant for multiple nonlinear optical processes, simultaneously satisfying phase matching for multiple processes is difficult task, but efficient enough that these multi-step optical parametric processes have benn demonstrated experimentally at Andrews et al 1970, Abu-Safe 2005)

Our interest is the process that one photon is annihilated and two photons are created.

$$
H_{NL} = \int d^3r \zeta^{(2)}_{ijl}(r) \hat{D}^+_i(r,t)\hat{D}^-_j(r,t)\hat{D}^-_l(r,t)
$$

We will be working on the paraxial regime so it is valid approximation to simply replace displacement field component indices with polarization indices since the component of the displacement field parallel to the $\vec{\epsilon}$.

## Hermite-Gaussian basis.

It will make calculations much simpler if we express the transverse momentum components of the field in terms of Hermite-Gaussian modes, since Gaussian pump beams and similar collection modes of down-converted light are valid descriptions of the light generated in SPDC experiments.

Let say $\vec{k}=\vec{q}+k_z \hat{z}$, where $\vec{q}$ is the projection of the momentum $\vec{k}$ onto the transverse plane.

we can express plane wave creation operator $\hat{a}^†_{\vec{q},k_z,s}$ as a sum over transverse mode creation operators $\hat{a}^†_{\vec{\mu},k_z,s}$, where $\mu$ is denoting 2D Hermite polynomial mode (n,m), ordered non-negative pair.

Thus,

$$
\hat{a}^†_{\vec{q},k_z,s} = \sum_{\mu}\tilde{C}_{\vec{q},\vec{\mu}}\hat{a}^†_{\vec{\mu},k_z,s}
$$

and 

$$
g_{\vec{\mu}}(x,y)=
\frac{1}{\sqrt{L_x L_y}}\sum_{\vec{q}}\tilde{C}_{\vec{\mu},\vec{q}}e^{-i\vec{q}\cdot\vec{r}}
$$

where we have defined $g_{\mu}(x,y)$ to be normalized Hermite-Gaussian wavefunction given by the index $\vec{\mu}$

$L_x$ and $L_y$ are x,y length of cavity for normalization.

Hermite-Gaussian approximation is well behaved when Hermite-Gaussian modes are encomppased by the crystal.

using an paraxial approximation (so that the frequency $w$ only depends on $k_z$), the displacement operator becomes:

$$
\hat{D}^-(\vec{r},t) = -i\sum_{\vec{\mu},k_z,s}\sqrt{\frac{\epsilon_0 n_{k_z}^2\hbar w_{k_z}}{2L_z}}\hat{\epsilon}_{k_z,s} g_{\mu}(x,y) e^{-i k_z z} \hat{a}^†_{\vec{\mu},k_z,s}e^{iwt}
$$

Here, $ \hat{a}^†_{\vec{\mu},k_z,s}e^{iwt}=\hat{a}^†_{\vec{\mu},k_z,s}(t)$

With $D$ operator and Non-linear Hamiltonian, we can handle SPDC process.

- We assume that pump light is classical light because pump field is bright enough.

- We assume that pump light is not diminished much due to down-conversion events (known as undepleted pump approximation)

## Classical pump light

Classical pump light can be written as 

$$
\vec{D}_p(\vec{r},t)=|D_p^0|\vec{\epsilon}_p f_p(\vec{r})\cos{(w_p t)}
$$

$\vec{\epsilon}_p$ : polarization of pump field, $f_p(\vec{r})$ : spatial function of light.

It can be separated into positive and negative frequency components:
$$
\vec{D}^+_p(\vec{r},t)=|D_p^0|\vec{\epsilon}_p f_p(\vec{r})\frac{e^{-iw_pt}}{2}
\newline
\vec{D}^-_p(\vec{r},t)=|D_p^0|\vec{\epsilon}_p f_p(\vec{r})\frac{e^{iw_pt}}{2}
$$

time averaged pump intensity is then :

$$
I_p = \frac{c}{2\epsilon_0 n^3}|D^0_p|^2|f_p(\vec{r})|^2
$$


## References

Introduction to the absolute brightness and number statistics in spontaneous parametric down-conversion

Why you should not use the electric field to quantize in nonlinear optics

BBO 크리스탈 같은 곳에 광자 하나가 들어가면 correlated photon 두개가 튀어나오는 현상.

![spdc.png](./img/spdc.png)

input photon (pumped photon), output photon (signal photon, idler photon)

만약 아웃풋 포톤 두개의 polarization 이 인풋과 같으면 type 0, 아웃풋 포톤 두개는 서로 같지만 인풋과는 orthogonal 하면 type 1, 그리고 아웃풋 포톤 두개가 서로 orthogonal 하면 (Horizontal 과 Vertical 처럼) type 2 SPDC.

$$
E\rightarrow\hat{E}=\hat{E}^+ +\hat{E}^-
$$

$$
H_{SPDC}= \int dr^3 \chi^{(2)}\hat{E}^+_p \hat{E}^-_s \hat{E}^-_i
$$