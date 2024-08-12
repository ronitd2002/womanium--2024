# Womanium coding Assignments for the 2024 cohort

## QBronze - Basics
QBronze is the basic module for Quantum algorithms and delas with basic arithmetic s=following quantum theory. Here's a breakdown of the quizzes :- 

## QNickel - Algorithms
QNickel is about basic Quantum algortihms namely Simon's algorithm, Deutsch-Josza algorithm , Grover's algorithm and it's use case for solving adder quantum circuits and solving MaxCut problems using Grover's algorithm which gives us the probability for 2 coloring graphs and the ways to generate unique points at the end of edges.

## QCobalt - Annealing
Using DWave's Ocean SDK in this module we solve Quadratic problems for optimization. The formulation of the same are enlisted in these exercise.

## Theory (Practical QC Implementations) [solutions]

### Quantum Annealing:

* What is quantum annealing?
  A quantum algorithm that utilizes the adiabatic theorem and has applications in optimization 

* What kind of qubits does D-Wave use?
  Superconducting flux qubits 

* How do we formulate real-world problems to solve on D-Wave’s quantum computers?
  Build a BQM by defining the variables and then combining an objective and constraints 

### Superconducting Quantum Hardware:

* How is quantum information encoded in a superconducting qubit, i.e. what constitutes the two-level system with defined states |0⟩ and |1⟩?
 * The phase difference across a Josephson junction.
 * The persistent current in a superconducting loop interrupted by Josephson junctions 
 * The charge distribution across a Josephson junction 

* How to initialize the superconducting qubit?
  * By cooling the qubit to extremely low temperature 

* How can we improve the coherence time of superconducting qubits?
  * By improving the design and materials that make up the qubits 

* How can we implement gates using superconducting qubits? (Hint: in classical computing we switch between 0 and 1 in a controlled way)
  * By applying tailored microwave pulses and control signals to the qubits 

* How is entanglement achieved in superconducting two-qubit gates?
  * Applying specific control pulses to turn on inter-qubit interactions 

* How do we differentiate between the qubit states for measurement in superconducting qubits?
  * By performing dispersive readout via a qubit-specific superconducting resonator 

* What are the most common sources of errors in superconducting quantum computing?
  * Errors in the initialization and measurement of qubit states 
  * Crosstalk between qubits and unintended interactions 
  * Imperfect materials that can absorb energy from the qubits 

* How are microwave resonators utilized in the implementation of superconducting qubits ? [wrong]

* Which of the following types of superconducting qubits are MOST COMMONLY used by large-scale quantum computing efforts?
  * Transmon qubits 

* State an advantage and a disadvantage of superconducting qubits as a quantum computing platform.
  * Advantage : Relatively fast operation.
  * Disadvantage : Decoherence time is very small.


### Silicon-based Quantum Hardware:

### Photonic Quantum Hardware:

### Neutral-Atom Quantum Hardware:


## Classiq - Quantum Algorithm Development. (Level 1)
Classiq Advanced Algorithms QC implementation. Minimal Circuit Depth, Circuit Optimization, Most Significant bit- Least significant bit exercises.

## Classiq - Quantum Algorithm Development. (Level 2)
Quantum Fourier Transform, Non unitary operations and Quantum Walk. Assignments are in jupyter notebook formats in the respective folder. A short summary is provided below against each.

## Pennylane - Quantum Machine Learning
Minimize the cost function (expval) with respect to test parameters for a custom variational circuit. Simple stuff. 

---

#### Project chosen for the Womanium cohort:- QML for Conspicutiy Detection (FRAUNHOFER)

Project specific `README.md` can be found in the respective directory.