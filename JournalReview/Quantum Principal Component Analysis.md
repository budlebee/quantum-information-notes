$$
Tr_\rho[e^{-iSt}\rho\otimes\sigma e^{iSt}]=Tr_\rho[(1-iSt)\rho\otimes\sigma(1+iSt)+O(t^2)]\newline
=Tr_\rho[\rho\otimes\sigma]-itTr_\rho[[S,\rho\otimes\sigma]] +Tr_\rho[O'(t^2)]

$$

$Tr_\rho$ traces out $\rho$. $[S,\rho\otimes\sigma]$ is commutation relation.

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

Thus, 

$$
Tr_\rho[\rho\otimes\sigma]-itTr_\rho[[S,\rho\otimes\sigma]] +Tr_\rho[O'(t^2)]\newline
=\sigma-it[\rho,\sigma]+Tr_\rho [O'(t^2)]\newline
\simeq (1-i\rho t)\sigma(1+i\rho t)\simeq e^{-i\rho t}\sigma e^{i\rho t}
$$

for infinitesimal time $t$.

By applying infinitesimal swap operation on $\rho\otimes\sigma$, we can construct unitary operator $e^{-i\rho t}$ 