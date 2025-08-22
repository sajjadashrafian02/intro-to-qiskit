Quantum Computing with Qiskit

This repo contains my practice work from the Coursera course Beginner’s Guide to Practical Quantum Computing with IBM Qiskit.

1. Overview

In this project, I use Qiskit to practice basic quantum computing concepts. I show you how to build circuits, use different gates, run simulations, and visualize important results.

2. Course Reference

* Course: Beginner’s Guide to Practical Quantum Computing with IBM Qiskit
* Platform: Coursera
* Provider: Packt Publishing & IBM Quantum

3. Topics Learned

The notebook covers  fundamental concepts, including:

* Qiskit basics: Importing, circuit creation, and visualization
* Initialization: Preparing qubits in arbitrary states
* Single-qubit gates:
  * Pauli gates (X, Y, Z)
  * Hadamard (H)
  * Phase and S/T gates
  * Rotation gates (Rx, Ry, Rz)
* Multi-qubit gates:
  * CNOT (CX)
  * Controlled operations (CH, CZ, etc.)
  * SWAP gate
* Analysis of quantum state:
  * Statevector simulation
  * Bloch sphere visualization
  * Probability distributions
* Measurement & results:
  * Running circuits on AerSimulator
  * Collecting counts
  * Plotting histograms
* Entanglement: Creating and measuring Bell states

4. Requirements

Install dependencies with:

pip install qiskit qiskit-aer matplotlib


Optional for advanced visualizations:

pip install qiskit-textbook


5. Usage

1. Clone the repository:

git clone https://github.com/yourusername/quantum-qiskit-course.git
cd quantum-qiskit-course


1. Open Jupyter Notebook:

jupyter notebook


1. Open the Jupyter Notebook file and execute each cell sequentially.

6. Example Outputs

Quantum Circuit Example

qc = QuantumCircuit(2)
qc.h(0)
qc.cx(0, 1)
qc.measure_all()
qc.draw("mpl")


Produces:
(circuit diagram placeholder)

Measurement Histogram

plot_histogram({'00': 512, '11': 512})


Shows probability distribution:
(histogram placeholder)

Bloch Sphere

plot_bloch_multivector(statevector)


Visualizes qubit states:
(Bloch sphere placeholder)

7. Acknowledgments

* Coursera & Packt Publishing for course material
* IBM Qiskit team for the open-source framework
* Matplotlib & NumPy for math and visualization tools

8. Next Steps

* Study the Quantum algorithm 
* Learn about quantum teleportation and quantum cryptography
* Try running circuits on real IBM Quantum hardware using the IBM Quantum tokens
