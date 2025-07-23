# Demonstrating Phase Kickback in Quantum Computing with Qiskit

## 🎯 Objective
Demonstrate the phase kickback phenomenon using a simple two-qubit quantum circuit in Qiskit, showing how a controlled phase rotation applied to the target qubit affects the control qubit.

## 📚 Theoretical Background
In quantum computing, when a control qubit is in superposition and a controlled gate (like `CRZ(θ)`) is applied, the phase can "kick back" from the target to the control. This highlights the unitary and reversible nature of quantum operations — a key distinction from classical computing.

## 🧪 Experiment Steps

1. Initialize a 2-qubit quantum circuit.
2. Apply `H` to the control qubit (superposition) and `X` to the target (sets it to |1⟩).
3. Apply a `CRZ(θ)` gate — phase affects only the target if control is |1⟩.
4. Apply a final `H` to the control — reveals the phase as a measurable difference.
5. Visualize the statevector and Bloch spheres.
6. Simulate and measure results using `AerSimulator`.

## 🧠 Why It Matters
Phase kickback is a key mechanism in:
- Quantum Phase Estimation (QPE)
- Shor’s Algorithm
- Quantum simulations

## 📊 Visualization
- Statevector amplitudes
- Bloch sphere representations
- Measurement histograms (with and without the final Hadamard)

## 📎 Additional Information
- Created by: Diego Saran
- License: MIT
- Version: 1.0
- Date: July 2025

## 🧰 Requirements
- Qiskit >= 2.1.0
- Qiskit IBM Runtime >= 0.40.0
- Matplotlib
- NumPy
