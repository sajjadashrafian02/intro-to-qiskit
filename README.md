# Quantum Computing with Qiskit

This repository contains my practice work from the Coursera course **Beginner’s Guide to Practical Quantum Computing with IBM Qiskit**.

## 1. Overview

In this project, I use **Qiskit** to practice basic quantum computing concepts. The notebook demonstrates how to:

* Build quantum circuits  
* Use different quantum gates  
* Run simulations  
* Visualize important results  

## 2. Course Reference

* **Course:** Beginner’s Guide to Practical Quantum Computing with IBM Qiskit  
* **Platform:** Coursera  
* **Provider:** Packt Publishing & IBM Quantum  

## 3. Topics Learned

The notebook covers fundamental concepts, including:

### 3.1 Qiskit Basics
* Importing Qiskit  
* Circuit creation  
* Circuit visualization  

### 3.2 Initialization
* Preparing qubits in arbitrary states  

### 3.3 Single-Qubit Gates
* Pauli gates (X, Y, Z)  
* Hadamard (H)  
* Phase and S/T gates  
* Rotation gates (Rx, Ry, Rz)  

### 3.4 Multi-Qubit Gates
* CNOT (CX)  
* Controlled operations (CH, CZ, etc.)  
* SWAP gate  

### 3.5 Analysis of Quantum State
* Statevector simulation  
* Bloch sphere visualization  
* Probability distributions  

### 3.6 Measurement & Results
* Running circuits on AerSimulator  
* Collecting counts  
* Plotting histograms  

### 3.7 Entanglement
* Creating and measuring Bell states  

## 4. Requirements

Install dependencies:

```bash
pip install qiskit-textbook
```
## 5. Usage

### 5.1 Clone the repository

```bash
git clone https://github.com/yourusername/quantum-qiskit-course.git
cd quantum-qiskit-course
```
## 5.3 Run the Notebook

Open the notebook file and execute each cell sequentially.

---

## 6. Example Outputs

### 6.1 Quantum Circuit Example

```python
from qiskit import QuantumCircuit

qc = QuantumCircuit(2)
qc.h(0)
qc.cx(0, 1)
qc.measure_all()
qc.draw("mpl")
```
**Produces:**  
![Circuit Diagram Placeholder](path/to/circuit-diagram.png)

---

## 6.2 Measurement Histogram

```python
from qiskit.visualization import plot_histogram

plot_histogram({'00': 512, '11': 512})
```
**Shows probability distribution:**  
![Histogram Placeholder](path/to/histogram.png)

---

## 6.3 Bloch Sphere

```python
from qiskit.visualization import plot_bloch_multivector

plot_bloch_multivector(statevector)
```
**Visualizes qubit states:**  
![Bloch Sphere Placeholder](path/to/bloch-sphere.png)

---

## 7. Acknowledgments

* Coursera & Packt Publishing for course material  
* IBM Qiskit team for the open-source framework  
* Matplotlib & NumPy for math and visualization tools  

---

## 8. Next Steps

* Study quantum algorithms  
* Learn about quantum teleportation and quantum cryptography  
* Run circuits on real IBM Quantum hardware using IBM Quantum tokens

