# 🧠 Quantum Computing Notes – IBM Basics of Quantum Information

---

## 1. Introduction
- What is quantum computing?
- Difference from classical computing:
  - Superposition
  - Entanglement
  - Measurement

---

## 2. Qubits and States
- Basis states: |0⟩, |1⟩
- Superposition: α|0⟩ + β|1⟩
- Bloch Sphere: (brief description)

---

## 3. Quantum Gates
### Single-Qubit Gates:
- X (NOT)
- H (Hadamard)
- Z
### Multi-Qubit Gates:
- CNOT

**Example (Qiskit):**
``python
from qiskit import QuantumCircuit
qc = QuantumCircuit(2)
qc.h(0)
qc.cx(0, 1)
qc.draw()

##4. Measurement
-Collapse to classical bit

-Syntax: qc.measure(q, c)

---


##5. Execution
Simulator vs real quantum device

Example:

python
Copy
Edit
from qiskit_aer import AerSimulator
result = AerSimulator().run(qc, shots=1024).result()
print(result.get_counts())
