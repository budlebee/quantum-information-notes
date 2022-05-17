For 2x2 system, P operator is pauli x matrix and T is defined by complex conjugation. 

A nontrivial example of a PT-symmetry Hamiltonian is 

$$
H=s\begin{bmatrix}
i\sin{\alpha} &1\\
1& -i\sin{\alpha}
\end{bmatrix}
$$
s and $\alpha$ is real number. s is a scaling constant and $\alpha$ is Hermiticity of $H$. When $\alpha=0$, Hamiltonian is a Hermitian. 

Eigenvalues are $E_{\pm}=\pm s\cos{\alpha}$, are real when $|\alpha|<\pi/2$.

Corresponding eigenstates are

$$
\ket{E_{+}(\alpha)}=\frac{e^{i\alpha/2}}{\sqrt{2\cos{\alpha}}}
\begin{bmatrix}1\\e^{-i\alpha}\end{bmatrix}
$$

$$
\ket{E_{-}(\alpha)}=\frac{ie^{-i\alpha/2}}{\sqrt{2\cos{\alpha}}}
\begin{bmatrix}1\\-e^{i\alpha}\end{bmatrix}
$$

These are not orthogonal each other in conventional quantum theory. 

Some useful formula as following:

$$
e^{i\phi\bold{\sigma\cdot \hat{n}}}=\cos{\phi}+i\sin{\phi}\bold{\sigma\cdot \hat{n}}
$$
where $\bold{\sigma}=(\sigma_0,\sigma_1,\sigma_2,\sigma_3)$ and $\bold{\hat{n}}$ is a normalized vector.

Our Hamiltonian is expressed as following:

$$
H=s\cos{\alpha}(\frac{\sigma_1+i\sin{\alpha}\sigma_3}{\cos{\alpha}}) = s\cos{\alpha}\bold{\sigma \cdot\hat{n}}
$$

Then time evolution is given by

$$
U(t)=e^{-itH}=e^{-its\cos{\alpha}\bold{\sigma \cdot\hat{n}}}=e^{-it'{\sigma \cdot\hat{n}}}
\newline
=\cos{t'}-i\sin{t'}{\sigma \cdot\hat{n}}
\newline
=\frac{1}{\cos{\alpha}}
\begin{bmatrix}
\cos{t'-\alpha}&-i\sin{t'}\\
i\sin{t'}&\cos{t'+\alpha}
\end{bmatrix} 
$$
where $\hbar=1$ for convinience.