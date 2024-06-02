## Quantum Non-Demolition Measurement (QND)

양자 상태를 어떤 특정 상태로 projection 시키면서 파괴하지 않고 알아내는 방법. 편광기반의 양자 상태는 포톤 디텍터가 광자를 흡수하면 해당 광자를 더 이상 사용할 수가 없는데, 초전도회로에서는 양자 상태를 0이나 1로 프로젝션 한 다음에도 양자상태가 0이나 1로 계속 유지가 된다.

## Dispersive Readout

트랜스몬 큐빗을 읽어내는 방법 중 하나. 트랜스몬 큐빗을 외부 resonator 와 캐패시터로 연결한다. 그 다음 resonator 에 주파수를 바꿔가며 스캔하면, 큐빗이 0 상태냐 1이냐에 따라 peak 주파수가 달라진다. 이를 통해 큐빗 상태를 0 또는 1로 프로젝션 시킬 수 있지만, 양자상태가 파괴되지는 않고 큐빗은 여전히 0 또는 1로 남아있게 된다.

### Jaynes-Cumming model

트랜스몬 큐빗 $\hbar \omega_q \sigma_z/2$ 과 외부 oscillating field $\hbar\omega_r a^\dagger a$ 사이의 커플링이 있을때 total excitation number 가 보존되는 Rotating-Wave approximation 해밀토니안은

$$
H \simeq \frac{1}{2}\hbar\omega_q \sigma_z +\hbar \omega_r a^\dagger a + \hbar g (\sigma_-a^\dagger + \sigma_+a)
$$

해당 해밀토니안은 $|e,n\rangle, |g,n+1\rangle$ 상태가 closed manifold 를 이룬다.

$$
\frac{H}{\hbar}|e,n\rangle = (n\omega_r +\frac{\omega_q}{2})|e,n\rangle +g\sqrt{n+1}|g,n+1\rangle \\ 
$$

$$
\frac{H}{\hbar} |g,n+1\rangle = g\sqrt{n+1}|e,n\rangle +[(n+1)\omega_r - \frac{\omega_q}{2}]|g,n+1\rangle
$$

n에 대한 2x2 해밀토니안을 행렬형태로 나타내면

$$
\frac{H}{\hbar} = (n+\frac{1}{2})\omega_r I_{2\times 2} +
\begin{pmatrix}
\frac{\triangle}{2} & g\sqrt{n+1}\\
g\sqrt{n+1}& - \frac{\triangle}{2}
\end{pmatrix}
$$

where $\triangle = \omega_q - \omega_r$

해당 해밀토니안의 eigenenergy 와 eigenstate 를 구하면,

$$
E_{\pm} = \left(n+\frac{1}{2}\right)\hbar\omega_r \pm \frac{\hbar}{2} \sqrt{\triangle^2 +4g^2 (n+1)}
$$
$$
|\psi_+\rangle = \cos{\left(\frac{\theta}{2}\right)}|e,n\rangle + \sin{\left(\frac{\theta}{2}\right)}|g,n+1\rangle \\
|\psi_-\rangle = -\sin{\left(\frac{\theta}{2}\right)}|e,n\rangle + \cos{\left(\frac{\theta}{2}\right)}|g,n+1\rangle
$$

where $\tan{\theta} = 2g\sqrt{n+1}/\triangle$.

### Dispersive regime

$\triangle \gg g$ 인 dispersive regime 에서, eigenenergy 와 해밀토니안을 up to first order 까지 binomial expansion 한다면

$$
E_{\pm} = \left(n+\frac{1}{2}\right)\hbar\omega_r \pm \frac{\hbar}{2} \sqrt{\triangle^2 +4g^2 (n+1)}\\
\simeq\left(n+\frac{1}{2}\right)\hbar\omega_r \pm \frac{\hbar \triangle}{2} \left[ 1+2\left( \frac{g}{\triangle} \right)^2(n+1)\right ]
$$

이때 totan excitation number $N_{ex} = a^\dagger a +\frac{\sigma_z+1}{2}$ 를 정의하면, eigenenergy 에 대응되는 해밀토니안은

$$
H\simeq \left(N_{ex}-\frac{1}{2}\right)\hbar\omega_r + \sigma_z \hbar\triangle \left[\frac{1}{2} + \left( \frac{g}{\triangle} \right)^2 N_{ex}\right]
$$

Dispersive shift $\chi = g^2/\triangle$ 을 정의하고, 에너지 오프셋을 무시한 해밀토니안을 쓰면 

$$
H_{disp} = \hbar(\omega_r +\chi \sigma_z)a^\dagger a +\frac{1}{2}\hbar(\omega_q +\chi)\sigma_z
$$

즉 큐빗의 상태가 $|e\rangle$ 이라면 resonator peak 이 $\omega_r+\chi$ 에서 나타나고, 큐빗의 상태가 $|g\rangle$ 이라면 resonator peak 이 $\omega_r-\chi$ 에서 나타난다. 큐빗 상태에 따라 resonator peak 이 달라지는 것을 이용해 큐빗 상태를 읽어내는 것을 dispersive readout 이라고 한다.