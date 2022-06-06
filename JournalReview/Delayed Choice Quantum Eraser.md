

correlated photons state from source as follows:

$$
\ket{\psi} = \frac{1}{\sqrt{2}}(\ket{U\nearrow}\ket{U\searrow}+\ket{L\nearrow}\ket{L\searrow})
$$

$U$ means photons created from upper slit and $D$ means photons created from lower slit. $\nearrow$ means photon that goes upwards(signal photon) and $\searrow$ means photon that goes downwards(idler photon).

Idlers photons meet some beam splitters and is directed to the four detectors. We get the state

$$
\ket{U\nearrow}(\frac{1}{2\sqrt{2}}\ket{1}+\frac{1}{2\sqrt{2}}\ket{2} +\frac{1}{2}\ket{4})\newline
+\ket{L\nearrow}(\frac{1}{2\sqrt{2}}\ket{1}+\frac{1}{2\sqrt{2}}\ket{2} +\frac{1}{2}\ket{3})
$$

If detector D4 is clicked, then state is $\ket{U\nearrow}$. This state has not interference property. 

But detector D1 is clicked, then state is $\frac{1}{\sqrt{2}}(\ket{U\nearrow}+\ket{L\nearrow})$. This state has a interference property.


## Conditional probabilities

Say we have two bipartite particles A and B and we want to measure observables $O_A$ and $O_B$. If we have corresponding eigenbases $\ket{i}_A$ and $\ket{j}_B$, we can write a general state as 

$$
\ket{\psi} = \sum_{i,j}\alpha_{ij}\ket{i}_A\ket{j}_B
$$

where $\sum|\alpha_{ij}|^2=1$.

When measuring $O_A$, the chance that the outcome $O_A$ equals the I-th eigenvalue $a_I$ is given by 

$$
P(O_A = a_I) = \sum_{j}|\alpha_{Ij}|^2
$$

And similar for $P(O_B = b_J)$. 

Say we have measured on B and got $O_B=b_J$, then the state becomes 

$$
\ket{\psi}\rightarrow\ket{\psi'}=\frac{\sum_i \alpha_{iJ}\ket{i}\ket{J}}{\sum_{i} |\alpha_{iJ}|^2}
$$

For this $\ket{\psi'}$ the chance to measure $O_A=a_I$ is 

$$
P(O_A=a_I|O_B=b_J)=\frac{|\alpha_{IJ}|^2}{\sum_i |\alpha_{iJ}|^2}
$$

The chance that $O_A=a_I$ and $O_B=b_J$ is

$$
P(O_A=a_I\cap O_B=b_J)=P(O_A=a_I|O_B=b_J)P(O_B=b_J) =|\alpha_{IJ}|^2 \newline
=P(O_B=b_J|O_A=a_I)P(O_A=a_I)
$$

The probability to find $O_A=a_I$ and $O_B=b_J$ does not depend on the relative order of measurements.