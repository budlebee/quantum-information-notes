# Five axioms of quantum mechanics

## State

A state is a complete description of a physical system. In Q.M, a state is a *ray* in a *Hilbert space*.

Hilbert space is 

- A vector space over the complex numbers $\mathbb{C}$

- It is defined inner prodcut $\braket{\phi|\psi}$ that maps an ordered pair of vectors to $\mathbb{C}$. 

- It is *complete* in the norm : $||\psi||=\braket{\psi|\psi}^{1/2}$. Completeness is an important proviso in infinite-dimensional function
spaces, since it ensures the convergence of certain eigenfunction expansions.

Ray is a like a vector, but vector has a direction and magnitude. But ray has a direction only.

## Observables

An observable is a property of a physical system that in principle can be measured. In Q.M, an observable is a self-adjoint operator (Hermitian)

An operator is a linear map taking verctors to vectors.

note: **AB+BA** and i(**AB-BA**) are always Hermitian if **A** and **B** are.

A Hermitian operator's eigenstates in a Hilber space form a complete orthonormal basis. We can express a Hermitian operator $A$ as
$$
A = \sum_{n} a_nE_{n}
$$
Here each $a_{n}$ is an eigenvalue of $A$ and $E_{n}$ is the corresponding orthogonal projection onto the space of eigenvectors with eigenvalue $a_{n}$.

The $E_{n}$ satisfy $E_{n}E_{m}=\delta_{n,m}E_{n}$ and $E^{\dagger}_{n}=E_{n}$

Alternative notation for the spectral representation of $A$ is

$$
A = \sum_{n}\ket{n}a_{n}\bra{n}
$$

where $\ket{n}$ is the orthonormal basis of eigenstates of $A$, with  $A\ket{n}=a_{n}\ket{n}$

(For unbounded operators in an infinite-dimensional space, the definition of Hermitian and the statement of the spectral theorem are more subtle, but this need not concern us)


## Measurement
 
A measurement is a process that information about the state of a physical system is acquired by observer.

If many identically prepared systems are measured, each described by the state $\ket{\psi}$, then the *expectation value* of the outcomes is

$$
\braket{a}=\sum_{n}a_{n}Prob(a_{n})=\sum_{n}a_{n}\bra{\psi}E_{n}\ket{\psi}=\bra{\psi}A\ket{\psi}
$$

## Dynamics

In QM, the time evolution of a closed system is described by a *unitray operator*

In the *Schrodinger picture*, initial time *t* and final time *t'*, state can be expressed as

$$
\ket{\psi (t')}=U(t',t)\ket{\psi (t)}
$$

where $U(t',t)$ is the unitary time evolution operator. If *H* is time independent, we may write *U(t',t)=\exp{-i(t'-t)H}*

## Composite Systems

Composite system of Hilbert space $\mathscr{H}_A$ and $\mathscr{H}_B$ is represented as tensor product $\mathscr{H}_A\otimes\mathscr{H}_B$.

State $\ket{\psi}_A$ in $\mathscr{H}_A$ and state $\ket{\phi}_B$ in $\mathscr{H}_B$ can be expressed as $\ket{\psi}_A\otimes\ket{\phi}_B$

The tensor product operator $M_{A}\otimes N_{B}$ is the operator that applies $M_{A}$ to system A and $N_{B}$ to system B. 

# The Qubit

quantum bit {0,1} is the unit of quantum information. It is a orthogonal vector in the 2 dimensional Hilbert space. 

General normalized state can be expressed as 

$$
a\ket{0}+b\ket{1}
$$
where $|a|^2+|b|^2=1$.

An important question is: what is the difference between a qubit and classical probabilistic bit?

In fact they are not the same for several reasons that we will explore. 

In a nutshell, there is only one way to look at a bit, but there is more than one way to look at a qubit.

# Spin 1/2

The coefficient a and b is more than just the probabilities of the outcomes of a measurement in the {0, 1} basis. The relative phase of a and b has physical significance.

A symmetry is a transformation that acts on a state, yet leaves all observable properties unchaged. In quantum mechanics, observations are measurements of Hermitian operators. If $A$ is measured in the state $\psi$, then $\ket{a}$ (the eigenvector of $A$) occurs with probability $|\braket{a|\psi}|^2$. A symmetry should leave these probabilities unchanged, when we rotate both the system and the apparatus if system has rotational symmetry.

A symmetry is a mapping of vectors in Hilber space $\ket{\psi}\rightarrow\ket{\psi'}$ that preserves the inner product values $|\braket{\phi | \psi}|=|\braket{\phi' | \psi'}|$ for all $\ket{\phi}$ and $\ket{\psi}$.

By Wigner's theorem, a mapping with this property can be chosen to be either unitary or anti-unitary by adopting suitable phase conventions.