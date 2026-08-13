# ⚛️ Quantum Mechanics Projects

A collection of undergraduate quantum mechanics projects focused on **quantum computing, optimization, and time-dependent quantum dynamics**.

The repository contains two final projects developed during my Physics studies at **Universidad de Antioquia**.

---

## 📂 Projects

### 1. Ising Model Using Quantum Computing and QAOA

Application of the **Quantum Approximate Optimization Algorithm (QAOA)** to a 2×2 Ising lattice.

The project combines analytical quantum mechanics, classical numerical optimization, and execution on real **IBM Quantum hardware**.

#### Topics
- Ising model
- QAOA
- Variational quantum algorithms
- Quantum circuits
- Classical optimization
- Qiskit
- IBM Quantum
- Quantum measurement
- Hardware noise

#### Main result

For the system studied:

- `J = 1`
- `h = 0.5`
- Optimal parameters: `γ ≈ 1.0`, `β ≈ 0.5`
- Ideal energy per site: `-1.5`
- IBM Quantum result: `≈ -1.4365`
- Ground state `|0000⟩` probability: `≈ 95.3%`

📄 **File:** `Ising_Model_QAOA_IBM_Quantum.pdf`

---

### 2. Quantum Dynamics in the Kramers–Henneberger Framework

Study of quantum systems interacting with **intense high-frequency electromagnetic fields** using the Kramers–Henneberger transformation.

The method transforms an explicitly time-dependent interaction into an effective problem involving an oscillating binding potential.

#### Topics
- Time-dependent quantum mechanics
- Strong-field physics
- Kramers–Henneberger transformation
- Effective Hamiltonians
- High-frequency approximation
- Perturbation theory
- Harmonic oscillator
- Anharmonic oscillator

The project shows how rapidly oscillating electromagnetic fields can modify the effective energy spectrum of a quantum system while suppressing transitions between states in the high-frequency regime.

📄 **File:** `Kramers_Henneberger_Quantum_Dynamics.pdf`

---

## 🛠️ Methods & Tools

`Quantum Mechanics` • `Python` • `Qiskit` • `IBM Quantum` • `SciPy` • `Numerical Optimization` • `Linear Algebra` • `Perturbation Theory`

---

## 📁 Repository Structure

```text
quantum-mechanics-projects/
│
├── Ising_Model_QAOA_IBM_Quantum.pdf
├── Kramers_Henneberger_Quantum_Dynamics.pdf
└── README.md
