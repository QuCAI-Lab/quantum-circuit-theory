<!-- Badges: -->
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?logo=paypal&style=flat-square)](https://www.paypal.me/CamponogaraViera/100)
![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20Windows-informational)
[![Python](https://img.shields.io/badge/Python-3.11.2-informational)](https://www.python.org/)
[![Contributions](https://img.shields.io/badge/contributions-welcome-orange?style=flat-square)](https://github.com/QuCAI-Lab/quantum-circuit-theory/pulls)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/QuCAI-Lab/quantum-circuit-theory/graphs/commit-activity)
[![License](https://img.shields.io/github/license/QuCAI-Lab/quantum-circuit-theory.svg?logo=CreativeCommons&style=flat-square)](https://github.com/QuCAI-Lab/quantum-circuit-theory/blob/dev/LICENSE.md)
<!-- [![Qiskit](https://img.shields.io/badge/Qiskit-0.42.1-6133BD)](https://qiskit.org/) -->
<!-- [![Pennylane](https://img.shields.io/badge/Pennylane-0.28.0-6133BD)](https://pennylane.ai/) -->

<!-- Logo: -->
<div align="center">
  <a href="https://qucai-lab.github.io/">
    <img src="https://github.com/QuCAI-Lab/qucai-lab.github.io/blob/main/assets/QuCAI-Lab.png" height="500" width="500" alt="Logo">
  </a>
</div>

<!-- Title: -->
<div align="center"> 
  <h1> Crash Course </h1>
  <h1> Quantum Circuit Theory </h1>
</div>

<!-- Author: -->
<div align="center">
  <b>Author: Lucas Camponogara Viera</a>
</div>

<!-- Dependencies: -->
# Dependencies
<a href="https://www.python.org/" target="_blank" rel="noopener noreferrer"><img height="27" src="https://www.python.org/static/img/python-logo.png"></a>
<a href="https://matplotlib.org" target="_blank" rel="noopener noreferrer"><img height="27" src="https://matplotlib.org/_static/images/logo2.svg"></a>
<a href="https://numpy.org/" target="_blank" rel="noopener noreferrer"><img height="27" src="https://numpy.org/images/logo.svg"></a>
<a href="https://sympy.org/" target="_blank" rel="noopener noreferrer"><img height="27" src="https://www.sympy.org/static/images/logo.png"></a>
<a href="https://scipy.org/" target="_blank" rel="noopener noreferrer"><img height="27" src="https://scipy.org/images/logo.svg"></a>
<a href="https://qiskit.org/" target="_blank" rel="noopener noreferrer">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://qiskit.org/documentation/stable/0.19/_static/logo.png">
    <img alt="Shows Qiskit logo for light color mode and dark color mode." src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Qiskit-Logo.svg/1200px-Qiskit-Logo.svg.png" height="27">
  </picture>
<a href="https://pennylane.ai/" target="_blank" rel="noopener noreferrer"><img height="27" src="https://pennylane.ai/img/logo.png"></a>
</a>
<br>

# Table of Contents

- **[00_postulates](notebooks/00_postulates.ipynb)**
	- Dirac notation
	- Postulate 1 (State Space)
	- Postulate 2 (Evolution)
	- Postulate 3 (Measurement)
		- Projective measurement (a.k.a von Neumann measurement) and Born's rule
		- Expectation value
	- 4 Postulate (Composite State)
	- System's dynamics: Schrödinger equation
	- Solution to the Schrödinger equation
- **[01_formalism](notebooks/01_formalism.ipynb)**
	- Linear operators.
	- Basis states.
		- Z-basis.
		- X-basis.
		- Y-basis.
	- Pauli group.
		- Pauli gates.
		- Pauli algebra.
	- Clifford group.
		- Clifford gates.
	- Hermitian gates.
	- Spectral decomposition theorem.
	- Operator function.
- **[02_single_qubit_gates](notebooks/02_single_qubit_gates.ipynb)**
	- Pauli gates.
	- Hadamard gate a.k.a superposition gate.
	- $R_{\hat{n}}(\theta)$ standard rotation single-qubit gate.
	- $P(\lambda)$ single-qubit phase gate.
		- Phase gate S.
		- Phase gate T.
	- $U(\alpha, \beta, \gamma, \delta)$ arbitrary single-qubit gate.
	- $U(\theta, \phi, \lambda)$ three-parameter single-qubit gate.
	- Qiskit $U1(\lambda)\equiv U(0,0,\lambda)=P(\lambda)$.
	- Qiskit $U2(\phi, \lambda) \equiv U(\pi/2, \phi, \lambda)$.
- **[03_change_of_basis.ipynb](notebooks/03_change_of_basis.ipynb)**
	- Measurement. 
	- From the $Z$-basis to the $X$-basis.
	- From the $Z$-basis to the $Y$-basis.
- **[04_two_qubit_gates](notebooks/04_two_qubit_gates.ipynb)**
- Deriving gates via spectral theorem, parity trick, and single-qubit rotations.
	- CNOT gate.
	- SWAP gate.
	- $ZZ(t)$ gate.
	- $XX(t)$ gate.
	- $YY(t)$ gate.
	- Verifying outer products.
- **[05_multi_qubit_gates](notebooks/05_multi_qubit_gates.ipynb)**
	- Multi-qubit gate $C_n^{j}(U_{2^m})$ with $n$ control qubits and $m$ target qubits.
- **[06_gate_identities](notebooks/06_gate_identities.ipynb)**
	- Pauli gates.
	- Standard rotation single-qubit gates.
	- Rotations.
	- Conjugation by Unitary.
- **[07_gate_decomposition](notebooks/07_gate_decomposition.ipynb)**
	- Pauli decomposition. 
	- Single-qubit gate decomposition.
	- Two-qubit gate decomposition.
- **[08_circuit_identities](notebooks/08_circuit_identities.ipynb)**
	- Qiskit little-endian convention.
	- Circuit identities via conjugation by unitary.
- **[09_universal_gate_set](notebooks/09_universal_gate_set.ipynb)**
	- Obtaining the universal gate set.
- **[10_trotterization](notebooks/10_trotterization.ipynb)**
	- The Trotter-Susuki formula
	- The Heisenberg XXX Spin-1/2 Lattice Model for $N=3$ Three Particles
	- Decomposition of $U_{\text{Heis3}}(t)$ using Trotterization
	- About the Trotterized Evolution
	    - Verifying identities with NumPy
	    - Verifying identities with Qiskit Opflow
- **[11_implementations](notebooks/11_implementations.ipynb)**
	- NumPy and Sympy implementations of:
		- Basis states.
		- Projector operators.
		- Single-qubit gates.
		- Two-qubit gates.
		- Eigenvalues and eigenvectors.
- **[algebraic_identities](notebooks/algebraic_identities.ipynb)**
	- Notation.
	- Representations.
	- Identities: algebraic proof of useful linear algebra identities for quantum circuits with SymPy and SciPy verification.
		- Retangular matrices.
		- Vectors.
		- Kronecker product between vectors.
		- Kronecker product between retangular matrices.
		- Kronecker product with vectors and matrices.
		- Commutation.
		- Matrix exponential.
		- Rotations.
- **[glossary](notebooks/glossary.ipynb)**
	- Jargon and Terminology.
- **[Q&A](notebooks/Q_A.ipynb)**
	- Questions and Answers.
  
# Conda Env.

1. Clone this repository and access the cloned directory:
```bash
git clone https://github.com/QuCAI-Lab/quantum-circuit-theory.git && cd quantum-circuit-theory
```
2. Create env.:
```bash
conda create -yn qct python==3.11.2 && conda activate qct
```
3. Install core dependencies:
```
python -m pip install -r requirements.txt
```

# References &nbsp; <a href="#"><img valign="middle" height="45px" src="https://img.icons8.com/book" width="45" hspace="0px" vspace="0px"></a> 

\[1] Nielsen MA, Chuang IL. 2010. "Quantum Computation and Quantum Information." New York: [Cambridge Univ. Press.](https://doi.org/10.1017/CBO9780511976667) 10th Anniv. Ed. 

\[2] Barenco, A., Bennett, C.H., Cleve, R., DiVincenzo, D.P., Margolus, N., Shor, P., Sleator, T., Smolin, J.A. and Weinfurter, H. (1995) Elementary gates for quantum computation. [Phys. Rev. A 52, 3457–3467](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.52.3457).

\[3] Scott Aaronson and Daniel Gottesman. 2004. Improved simulation of stabilizer circuits. [Phys. Rev. A 70, 5](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.70.052328) (Nov. 2004),
052328.

\[4] John Preskill. "Course Information for Physics 219/Computer Science 219 Quantum Computation." [California Institute of Technology](http://theory.caltech.edu/~preskill/ph229/).
- Chapter 5: Classical and Quantum Circuits.

\[5] Hans J. Weber and George B. Arfken. Essential Mathematical Methods for Physicists. [Academic Press, NY](https://g.co/kgs/RFBRhf).

# License

This work is licensed under a [Creative Commons Zero v1.0 Universal](LICENSE.md) license.

<hr>

Created and maintained by [@camponogaraviera][1].

[1]: https://github.com/camponogaraviera
