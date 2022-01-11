
# Entanglement Swap

assume entangled state
$$
\ket{\Phi^+}_{AB}\ket{\Phi^+}_{CD} 
= \frac{1}{2}(\ket{0}_{A}\ket{00}_{BC}\ket{0}_{D}  
+ \ket{0}_{A}\ket{01}_{BC}\ket{1}_{D}
\newline
 + \ket{1}_{A}\ket{10}_{BC}\ket{0}_{D} + \ket{1}_{A}\ket{11}_{BC}\ket{1}_{D})
$$

Bell State Measurement (BSM) for $\ket{\Phi^+}_{BC}$ is, $$I\otimes \bra{\Phi^+}_{BC}\otimes I$$

then,

$$
I\otimes \bra{\Phi^+}_{BC}\otimes I\ket{\Phi^+}_{AB}\ket{\Phi^+}_{CD}
\newline
= \frac{1}{2\sqrt{2}}[
    \ket{0}(\braket{00|00}+\braket{11|00})\ket{0}
    \newline
    +\ket{0}(\braket{00|01}+\braket{11|01})\ket{1}
    \newline
    +\ket{1}(\braket{00|10}+\braket{11|10})\ket{0}
    \newline
    +\ket{1}(\braket{00|11}+\braket{11|11})\ket{1}
 ] 
$$
$$
= \frac{1}{2\sqrt{2}}[\ket{00}_{AD}+\ket{11}_{AD}] = \frac{1}{2}\ket{\Phi^+}_{AD}
$$
By Meaeusring BC, we can get entangled state AD. It is called Entanglement Swap.

# Quantum Memory

We need memory to store quantum state. We store quantum state using atomic state and send quantum state using photon state. So, we need atom-photon coupling. 

![stokes_process](./stokes_process.png)

