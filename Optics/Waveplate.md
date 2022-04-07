# Waveplate

slow axis vertical, fast axis horizontal 의 경우

horizontal axis 기준으로 $\theta$ 만큼 돌렸을때의 편광 상태 구하기

$$
HWP(0) =\begin{pmatrix}
e^{-i\pi/2} & 0 \\
 0 & e^{i\pi/2}
\end{pmatrix} =e^{-i\pi/2}\begin{pmatrix}
1 & 0 \\
 0 & -1
\end{pmatrix} 
$$

$$
QWP(0) =\begin{pmatrix}
e^{-i\pi/4} & 0 \\
 0 & e^{i\pi/4}
\end{pmatrix} =e^{-i\pi/4}\begin{pmatrix}
1 & 0 \\
 0 & i
\end{pmatrix} 
$$

이고, $\theta$만큼 좌표변환을 하는 변환행렬은

$$
R(\theta)=\begin{pmatrix}
cos{\theta} & sin{\theta} \\
-sin{\theta} & cos{\theta}
\end{pmatrix}
$$

이므로, 
$$
HWP(\theta) = R(\theta)HWP(0)R(-\theta) = e^{-i\pi/2}\begin{pmatrix}
cos{2\theta} & sin{2\theta} \\
sin{2\theta} & -cos{2\theta}
\end{pmatrix}
$$

$$
QWP(\theta) = R(\theta)QWP(0)R(-\theta) = e^{-i\pi/4}\begin{pmatrix}
cos^2{\theta}+isin^2{\theta} & (1-i)sin{2\theta} \\
(1-i)sin{2\theta} & icos^2{\theta}+sin{\theta}
\end{pmatrix}
$$
