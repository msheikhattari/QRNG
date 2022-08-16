# Quantum State Tomography

### Classical Tomography
**Tomography** is the process of imaging using sectioning. An example in medicine is the CT (computerized tomography) scan, which creates a 3D picture from a series of 2D xray scans of different angles of your body.

### Quantum State Tomography
In quantum physics, tomography refers to the reconstruction of a quantum state using measurements of an ensemble of identical quantum states. In order to uniquely identify the state, the measurements must be **tomographically complete**, meaning that the measured operators must form an operator basis on the Hilbert space of the system.
- Think of it like working backward's using **Born's rule**. Usually we have the wavefunction and square it to get a probability distribution. Instead we use the measurement results to infer probabilities, which are then used to determine a density matrix which best fits the observations.

### Methods of quantum state tomography
1. Born's rule: the simplest form of quantum tomography can be derived using Born's rule, as described above, but it relies on being in a known pure state. 
2. Linear inversion: for a general mixed state, we use the following technique. We can construct a column vector with all of the measurement probabilties from before, let's call it $\vec{p}$. Another matrix, call it $A$, is defined as $\begin{pmatrix} \vec{E}_1^\dagger \\ \vec{E}_2^\dagger \\ \vec{E}_3^\dagger \\ \vdots \end{pmatrix}$, where $E_i$ is a fixed list of individual measurements; $A$ does all the measurements at once, such that $A\vec{\rho} = \vec{p}$. Linear inversion corresponds to inverting this system using $\vec{p}$ to derive $\vec{\rho}$ (which is isomorphic to $\rho$). Since the system is not going to be square in general, we perform the following trick: $A^TA\vec{\rho} = A^T\vec{p}$; $\vec{\rho} = (A^TA)^{-1}A^T\vec{p}$.  This only works if the measurement list $E_i$ is tomographically complete, otherwise $A^TA$ will not be invertible. 
3. Other methods exist, these are tools in probability. https://en.wikipedia.org/wiki/Quantum_tomography 