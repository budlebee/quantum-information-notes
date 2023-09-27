## Nonlinear Wave Equation

Maxwell equation in SI unit

1. $\nabla\cdot \vec{D}=\rho$
2. $\nabla\cdot \vec{B}=0$
3. $\nabla\times \vec{E}=-\frac{∂\vec{B}}{∂t}$
4. $\nabla\cdot \vec{H}= \frac{∂\vec{D}}{∂t} +\vec{J}$

Assumption : no free sources ($\rho=0$, $\vec{J}=0$) and no magnetic property ($B=\mu_0 H$)

Let take curl on equation 3:

$$
\nabla\times\nabla\times \vec{E} = -\frac{∂}{∂t}\nabla \times \vec{B}=-\mu_0\frac{∂^2 \vec{D}}{∂t^2}
$$

by $\nabla\times(\nabla\times \vec{E})=\nabla(\nabla\cdot\vec{E})-\nabla^2 \vec{E}$, and we assume that $\vec{E}$ field does not vary quickly at propagate direction:  $\nabla(\nabla\cdot\vec{E})\simeq0$.

$$
\nabla^2 \vec{E}-\frac{1}{\epsilon_0 c^2}\frac{∂\vec{D}}{∂t^2} = 0
$$

Let split the induced polarization $\vec{P}$ into linear term and nonlinear term

$$
\vec{P}=\vec{P}^{(1)}+\vec{P}^{NL}
$$

Displacement vector also can be represented in a similar way:

$$
\vec{D}=\vec{D}^{(1)}+\vec{P}^{NL}
$$

where $\vec{D}^{(1)} = \epsilon_0 \vec{E}+\vec{P}^{(1)}$

Therefore, nonlinear wave equation is:

$$
\nabla^2 \vec{E}-\frac{1}{\epsilon_0 c^2}\frac{∂\vec{D}^{(1)}}{∂t^2} = \frac{1}{\epsilon_0 c^2}\frac{∂^2\vec{P}^{NL}}{∂t^2}
$$

### Frequency-mode Generalization

$$
\vec{E}(\vec{r},t)=\sum_n \vec{E}_n(\vec{r},t) \\
\vec{D}^{(1)}(\vec{r},t)=\sum_n \vec{D}_n^{(1)}(\vec{r},t) \\
\vec{P}^{NL}(\vec{r},t)=\sum_n \vec{P}^{NL}_n(\vec{r},t) \\
$$

where 

$$
\vec{E}_n(\vec{r},t) =\vec{E}_n(\vec{r})e^{-iw_n t} +c.c.\\
\vec{D}_n^{(1)}(\vec{r},t)=\vec{D}_n^{(1)}(\vec{r})e^{-iw_n t} +c.c.\\
\vec{P}^{NL}_n(\vec{r},t) = \vec{P}^{NL}_n(\vec{r})e^{-iw_n t}+c.c.
$$

Since $P^{(1)}_i = \epsilon_0\chi_{ij}^{(1)}E_j$, we can represent $D^{(1)}$ using dielectric tensor

$$
\vec{D}^{(1)}_n(\vec{r}) = \epsilon_0 \overleftrightarrow{\epsilon}^{(1)}(w_n)\cdot\vec{E}_n(\vec{r})
$$

So, nonlinear wave equation becomes:

$$
\nabla^2 \vec{E}_n(\vec{r})+\frac{w^2_n}{ c^2}\overleftrightarrow{\epsilon}^{(1)}(w_n) \cdot\vec{E}_n(\vec{r})= -\frac{w_n^2}{\epsilon_0 c^2}\vec{P}_n^{NL}(\vec{r})
$$

Frequency domain wave equation. It is often referred to as a Helmholtz equation.


## Reference

Boyd nonlinear optics 4th Ch 2.1