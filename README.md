# Quantum Mechanics Projects

A collection of advanced undergraduate projects in **quantum mechanics and quantum computing**, focused on analytical derivations, numerical methods, variational algorithms, and quantum dynamics under time-dependent electromagnetic fields.

The repository contains two main projects:

1. **Ising Model Using Quantum Computing and QAOA**
2. **Quantum Dynamics in the Kramers–Henneberger Framework**

---

## ⚛️ 1. Ising Model Using Quantum Computing and QAOA

This project studies the **Ising model** from a quantum-computing perspective using the **Quantum Approximate Optimization Algorithm (QAOA)**.

The goal is to use a hybrid quantum-classical algorithm to find low-energy configurations of a (2\times2) Ising lattice.

### Main topics

* Ising Hamiltonian
* Pauli (X) and (Z) operators
* Computational basis states
* QAOA cost operator
* QAOA mixer operator
* Variational quantum states
* Classical parameter optimization
* Quantum circuit implementation
* IBM Quantum hardware
* Measurement statistics
* Noise in real quantum devices

The Ising Hamiltonian is written as

[
H_{\mathrm{Ising}}
==================

-J\sum_{\langle i,j\rangle} Z_i Z_j
-h\sum_i Z_i.
]

The QAOA state depends on two variational parameters,

[
|\psi(\gamma,\beta)\rangle
==========================

U(\beta,X),
U(\gamma,C),
H^{\otimes N}|0\rangle^{\otimes N}.
]

A classical optimizer is then used to minimize the expected energy

[
F(\gamma,\beta)
===============

\langle\psi(\gamma,\beta)|
H_{\mathrm{Ising}}
|\psi(\gamma,\beta)\rangle.
]

### Results

For the studied (2\times2) lattice with

[
J=1,
\qquad
h=0.5,
]

the classical optimization gives approximately

[
\gamma^*\approx1.0,
\qquad
\beta^*\approx0.5.
]

The optimized circuit was also executed on **IBM Quantum hardware**.

The best experimental point produced an energy per site of approximately

[
\frac{\langle C\rangle_{\mathrm{IBM}}}{N}
\approx -1.4365,
]

compared with the ideal value

[
\frac{\langle C\rangle_{\mathrm{ideal}}}{N}
=-1.5.
]

The ground-state configuration

[
|0000\rangle
]

was measured with a probability of approximately

[
P(0000)\approx95.3%.
]

The difference between the ideal and experimental results illustrates the effects of **hardware noise, gate errors, measurement errors, and finite sampling**.

---

## 🌊 2. Quantum Dynamics in the Kramers–Henneberger Framework

This project studies a quantum system interacting with an **intense, high-frequency electromagnetic field**.

Instead of solving the explicitly time-dependent Schrödinger equation directly, the problem is transformed into an accelerated reference frame using the **Kramers–Henneberger transformation**.

The original Hamiltonian in the length gauge is

[
H_L(t)
======

\frac{p^2}{2m}
+
V(\mathbf r)
------------

q,\mathbf r\cdot\mathbf E(t),
]

with

[
\mathbf E(t)
============

E_0\cos(\omega t)\hat{\mathbf e}.
]

The classical displacement produced by the field is described by

[
m\ddot{\boldsymbol{\alpha}}(t)
==============================

q\mathbf E(t).
]

After transforming to the accelerated frame, the Hamiltonian becomes

[
H_{\mathrm{KH}}(t)
==================

\frac{p^2}{2m}
+
V\big(\mathbf r+\boldsymbol{\alpha}(t)\big).
]

This formulation removes the explicit dipole interaction and replaces it with a **time-dependent displacement of the binding potential**.

---

## High-frequency approximation

The displaced potential is separated into an average contribution and an oscillating contribution,

[
V(\mathbf r+\boldsymbol{\alpha}(t))
===================================

\overline{V}*{\mathrm{KH}}(\mathbf r)
+
\Delta V*{\mathrm{KH}}(\mathbf r,t).
]

The effective Hamiltonian is therefore approximated by

[
H_{\mathrm{KH}}^{\mathrm{eff}}
==============================

\frac{p^2}{2m}
+
\overline{V}_{\mathrm{KH}}(\mathbf r).
]

The remaining term

[
\Delta V_{\mathrm{KH}}(\mathbf r,t)
]

can be treated as a time-dependent perturbation.

In the high-frequency regime, transition amplitudes associated with this oscillating contribution are suppressed roughly as

[
c_m^{(1)}
\sim
\frac{
\langle m|\Delta V_{\mathrm{KH}}|n\rangle
}{
\hbar\omega
}.
]

---

## Harmonic oscillator example

For a harmonic potential,

[
V(x)
====

\frac12m\Omega^2x^2,
]

the averaged KH potential becomes

[
\overline{V}_{\mathrm{KH}}(x)
=============================

\frac12m\Omega^2x^2
+
\frac14m\Omega^2\alpha_0^2.
]

The main effect is therefore a constant energy shift,

[
\Delta E
========

\frac14m\Omega^2\alpha_0^2.
]

The eigenstates remain those of the ordinary harmonic oscillator.

---

## Anharmonic oscillator example

For

[
V(x)
====

\frac12m\Omega^2x^2
+
\lambda x^4,
]

the KH averaging modifies the curvature of the effective potential.

The effective frequency satisfies

[
\Omega_{\mathrm{eff}}^2
=======================

\Omega^2
+
\frac{6\lambda\alpha_0^2}{m}.
]

For

[
\lambda>0,
]

the effective confinement becomes stronger and the internal energy spectrum is modified.

---

## 🧠 Main concepts explored

This repository covers topics including:

* Quantum mechanics
* Quantum computing
* Variational quantum algorithms
* QAOA
* Ising model
* Quantum optimization
* IBM Quantum
* Qiskit
* Pauli operators
* Quantum measurement
* Time-dependent quantum mechanics
* Strong-field physics
* Kramers–Henneberger transformation
* High-frequency approximations
* Perturbation theory
* Harmonic and anharmonic oscillators

---

## 📂 Repository Structure

```text
quantum-mechanics-projects/
│
├── Ising_Model_QAOA_IBM_Quantum.pdf
├── Kramers_Henneberger_Quantum_Dynamics.pdf
└── README.md
```

---

## 🎯 Purpose

The purpose of this repository is to explore two complementary areas of modern quantum physics:

**Quantum computation and optimization**, through QAOA applied to the Ising model,

and

**time-dependent quantum dynamics**, through the Kramers–Henneberger description of systems interacting with intense electromagnetic fields.

Together, the projects combine

**Quantum Mechanics + Mathematical Physics + Numerical Optimization + Quantum Computing + Strong-Field Physics**.
