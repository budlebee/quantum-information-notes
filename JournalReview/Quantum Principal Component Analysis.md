$$
Tr_\rho[e^{-iS\triangle t}\rho\otimes\sigma e^{iS\triangle t}]=Tr_\rho[(1-iS\triangle t)\rho\otimes\sigma(1+iS\triangle t)+O(\triangle t^2)]\newline
=Tr_\rho[\rho\otimes\sigma]-i\triangle tTr_\rho[[S,\rho\otimes\sigma]] +Tr_\rho[O'(\triangle t^2)]

$$

$Tr_\rho$ traces out $\rho$. $[S,\rho\otimes\sigma]$ is commutation relation.


Thus, 

$$
Tr_\rho[\rho\otimes\sigma]-i\triangle tTr_\rho[[S,\rho\otimes\sigma]] +Tr_\rho[O'(\triangle t^2)]\newline
=\sigma-i\triangle t[\rho,\sigma]+Tr_\rho [O'(\triangle t^2)]\newline
\simeq (1-i\rho \triangle t)\sigma(1+i\rho\triangle  t)\simeq e^{-i\rho\triangle  t}\sigma e^{i\rho\triangle  t}
$$

for infinitesimal time $\triangle t$. Swap operator S is sparse matrix (almost components are zero) and can be performed efficiently. By performing $e^{-iS\triangle t}$ on $\rho\otimes\sigma$ repeatedly, we can get  $ e^{-i\rho n\triangle  t}\sigma e^{i\rho n\triangle  t}$

By applying infinitesimal swap operation on $\rho\otimes\sigma$, we can construct unitary operator $e^{-i\rho t}$ .


$\ket{\chi_i}$ is a eigenstate of $\rho$ and of $e^{-i\rho t}$. 
$$
\rho = \sum_i r_i\ket{\chi_i}\bra{\chi_i}
 \newline
\rho\ket{\chi_i} =r_i\ket{\chi_i}\newline
e^{-i\rho t}\ket{\chi_i} = e^{-ir_i t}\ket{\chi_i}
$$

For Quantum Phase Estimation (QPE), $U^{2^t}\ket{u} = e^{2\pi i2^{t} \phi}\ket{u}$.

varying time t, infinitesimal swap operation is QPE process. $\ket{t}\ket{\chi}\rightarrow \ket{t}e^{-i\rho t}\ket{\chi}=\ket{t}e^{-ir t}\ket{\chi}$


the unitary operator $\sum_{n}\ket{n\triangle t}\bra{n\triangle t}\otimes\prod_{j=1}^{n}e^{-iS_j \triangle t}$ to $\ket{n\triangle t}\bra{n\triangle t}\otimes\sigma\otimes\rho ...\otimes\rho$

QPE yields the state $\sum_{i}r_i \ket{\chi_i}\bra{\chi_i}\otimes \ket{r_i} \bra{r_i}$


## additional note

For a single qubit density matrix,

$$
\rho\otimes\sigma=\begin{bmatrix}
\rho_{11}\begin{bmatrix}
\sigma_{11}&\sigma_{12}\\
\sigma_{21}&\sigma_{22}
\end{bmatrix}&&
\rho_{12}\begin{bmatrix}
\sigma_{11}&\sigma_{12}\\
\sigma_{21}&\sigma_{22}
\end{bmatrix} \\
\rho_{21}\begin{bmatrix}
\sigma_{11}&\sigma_{12}\\
\sigma_{21}&\sigma_{22}
\end{bmatrix}&&
\rho_{22}\begin{bmatrix}
\sigma_{11}&\sigma_{12}\\
\sigma_{21}&\sigma_{22}
\end{bmatrix}
\end{bmatrix}
$$

$$
S\rho\otimes\sigma=\begin{bmatrix}
\rho_{11}\sigma_{11}&\rho_{11}\sigma_{12}&\rho_{12}\sigma_{11}&\rho_{12}\sigma_{12}\\
\rho_{21}\sigma_{11}&\rho_{21}\sigma_{12}&\rho_{22}\sigma_{11}&\rho_{22}\sigma_{12}\\
\rho_{11}\sigma_{21}&\rho_{12}\sigma_{22}&\rho_{11}\sigma_{21}&\rho_{12}\sigma_{22}\\
\rho_{21}\sigma_{21}&\rho_{22}\sigma_{22}&\rho_{21}\sigma_{21}&\rho_{22}\sigma_{22}
\end{bmatrix}
$$

$$
\rho\otimes\sigma S=\begin{bmatrix}
\rho_{11}\sigma_{11}&\rho_{12}\sigma_{12}&\rho_{11}\sigma_{11}&\rho_{12}\sigma_{12}\\
\rho_{11}\sigma_{11}&\rho_{12}\sigma_{12}&\rho_{11}\sigma_{11}&\rho_{12}\sigma_{12}\\
\rho_{21}\sigma_{21}&\rho_{22}\sigma_{22}&\rho_{21}\sigma_{21}&\rho_{22}\sigma_{22}\\
\rho_{21}\sigma_{21}&\rho_{22}\sigma_{22}&\rho_{21}\sigma_{21}&\rho_{22}\sigma_{22}
\end{bmatrix}
$$

$$
Tr_\rho[\rho\otimes\sigma] = \begin{bmatrix}
(\rho_{11}+\rho_{22})\sigma_{11}&(\rho_{11}+\rho_{22})\sigma_{12}\\
(\rho_{11}+\rho_{22})\sigma_{21}&(\rho_{11}+\rho_{22})\sigma_{22}\\
\end{bmatrix}
$$