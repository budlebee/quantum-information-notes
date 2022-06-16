## superposition of two waves

Consider a superposition of two waves:

$$
\psi_1(x,t) = Ae^{i(kx-wt)}\newline
\psi_2(x,t) = Ae^{i((k+\Delta k)x-(w+\Delta w)t)}\newline
\psi = \psi_1 + \psi_2
$$

where $\Delta k$ and $\Delta w$ are small quantity.

Real part of $\psi$ is as follows:

$$
A[\cos{(kx-wt)}+\cos{(kx-wt)}\cos{(\Delta kx-\Delta wt)} - \sin{(kx-wt)}\sin{(\Delta kx-\Delta wt)}]
$$

It can be rewritten as follows by trigonometric function formulae

$$
\psi_{real}=2A\cos{(\frac{\Delta k x - \Delta w t}{2})}\cos{((k+\frac{\Delta k}{2})x-(w+\frac{\Delta w}{2})t)}
$$

Left cosine function is envelope. 

## superposition of n waves

Consider a superposition of n waves and get a limit $n\rightarrow \infty$

$$
\psi(x,t) = \sum_{s=1}^{n} A_s e^{i(k_s x -w_s t)} \newline

\rightarrow \int_{-\infty}^{\infty}A(k)e^{i(kx-w(k)t)}
$$

expand $w(k)$ up to first order, then

$$
w(k) = w(k_0) + \frac{dw}{dk}\times(k-k_0)+... = w_0+w_0'\times(k-k_0)+...
$$

$$
kx-wt = k_0 x - k_0 x + kx -w_o t -w_0' (k-k_0)t\newline

= (k_0 x - w_0 t) + (k-k_0)(k-w_0' t)
$$

$$
\psi(x,t) = \int_{-\infty}^{\infty} A(k)e^{i(k-k_0)(x-w_0't)}e^{i(k_0 x-w_0 t)}dk
$$

$e^{i(k-k_0)(x-w_0't)}$ part is effective amplitude that varies smoothly.

If effective amplitude phase is constant, 

$$
x-w_0't = const\newline

dx - w_0'dt = 0\newline

\frac{dx}{dt} = w_0' = \frac{dw}{dk} \equiv v_g 
$$

Phase velocity $v=w/k$, so $k=w/v$.

$$
\frac{1}{v_g}=\frac{d}{dw}(w/v)|_0 = \frac{v_0 - wdv/dw|_0}{v_0^2} \newline

v_g = \frac{v_0}{1-\frac{w_0}{v_0}dv/dw|_0}
$$

In non-dispersive media, $dv/dw=0$, so $v_g=v$
