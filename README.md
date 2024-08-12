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
  * A quantum algorithm that utilizes the adiabatic theorem and has applications in optimization 

* What kind of qubits does D-Wave use?
  * Superconducting flux qubits 

* How do we formulate real-world problems to solve on D-Wave’s quantum computers?
  * Build a BQM by defining the variables and then combining an objective and constraints 

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

* How is quantum information encoded in a silicon qubit, i.e. what constitutes the two-level system with defined states |0⟩ and |1⟩?
  * Information is encoded in the spin of the electron (residing in the potential well of a donor nucleus or quantum dot) or the spin of the donor nucleus 

* How to initialize the silicon qubit?
  *  The electron is initialized by tuning the Fermi level of a single electron transistor to lie between the electron spin up and spin down energy levels . Only a spin down electron (|0⟩ state) will have enough energy to tunnel from the single electron transistor 

* How can we improve the coherence time of silicon qubits?
  * Isotopically enrich the silicon to remove 29Si nuclear spins 
  * Increase the temperature of the dilution refrigerator to 1 K 
  * Increase the strength of the external magnetic field 

* How can we implement gates using silicon qubits? (Hint: in classical computing we switch between 0 and 1 in a controlled way)
  * We use an on-chip microwave antenna to supply an oscillating magnetic field at a frequency resonant with the energy gap between the spin down and spin up states to drive between the |0⟩ and |1⟩ states.

* Two qubit gates use entanglement. How can we entangle two spatially-separated donor spin qubits?
  *   Two flip flop qubits (created by the antiparallel spin states of a donor nucleus and electron) can be coupled by the electric dipole interaction when each electron is pulled away from its donor nucleus 
  * Two donor nuclear spins can be entangled through their hyperfine interaction with a shared electron spin 
  * Two electron spins can be entangled through the exchange interaction if the electron wavefunctions are close enough together to overlap with each other 

* How do we differentiate between the qubit states for measurement?
  * A spin up electron (|1⟩ state) will tunnel onto a single electron transistor island causing the current flowing through the single electron transistor to change due to the altered charge environment. A spin down electron (|0⟩ state) will not have enough energy to tunnel onto the single electron transistor island, leaving the SET current unchanged .

* What are the most common sources of errors in silicon-based quantum computing?
  * Electric field noise caused by two-level fluctuators in the environment (e.g charge traps at the oxide interface) result in decoherence 
  * Over or under-rotation of the quantum gates will introduce errors into your quantum circuit.
  * $^{29}Si$ nuclear spins in the environment decrease the coherence time of the electron spin by contributing to magnetic field noise. 

* What is an advantage of using a heavier group V donor over the standard phosphorus donor?
  * Heavier donors have higher nuclear spin, providing a larger Hilbert space (with more energy levels) with the potential of encoding a qudit or multiple qubits 

* How can spin qubits be fabricated in silicon?
  * Quantum dots can be defined by accumulating electrons under the oxide interface using on-chip electric gates, patterned using electron beam lithography 
  * Donor atoms can be placed inside the silicon crystal lattice using a scanning tunneling microscope lithography, phosphine dosing and silicon encapsulation. The donor provides both a nuclear and electron spin 
  * Donor atoms can be inserted into the silicon crystal lattice using ion implantation and annealing to repair the crystal. The donor provides both a nuclear and electron spin 

  (All of the above, depending on whether you want a donor spin qubit or just an electron spin qubit )

* State an advantage and a disadvantage of silicon-based qubits as a quantum computing platform. 
  * Advantage: Smallest qubits (50 nm), so can fit a full useful quantum processor on a single chip; Qubits can be moved around; Can tolerate heating effects; Errors are easier to correct (biased errors).
  * Disadvantage: Small size requires state-of-the-art manufacturing partners; Tolerance to materials defects is low; requirement for advanced fabrication reflects in late onset for qubit count.

### Photonic Quantum Hardware:

* How is quantum information encoded in a photonic qubit, i.e. what constitutes the two-level system with defined states  |0⟩  and  |1⟩ ?
  * The information is encoded into two orthogonal grid-states in the phase space of light. 

* How to initialize the photonic qubit?[wrong]
 
* How can we improve the coherence time of photonic qubits?
  * By decreasing phase noise in the system. 
 
* How can we implement gates using photonic qubits? (Hint: in classical computing we switch between 0 and 1 in a controlled way)
  * Measurement-induced teleportation in a cluster state. 

* How do we create two-qubit gates use entanglement?
  * Measurement-induced teleportation in a cluster state. 

* How do we differentiate between the qubit states for measurement?
  * Measuring one of the quadratures of the light.

* What are the most common sources of errors in photonic quantum computing? [wrong]

* How is squeezed light generated?
  * Via nonlinear interactions with polarizable media. 

* What is the advantage to using GKP-based cluster-state computing compared to fusion-based cluster-state computing? [wrong]

* State an advantage and a disadvantage of photons as a quantum computing platform.
  * Advantages: All-to-all connectivity; Photonic waveguides are relatively large and easy to fabricate.
  * Disadvantage: Tolerance to detector imperfections is low; Number of qubits in a single chip is very limited; Uses non-standard computation method (one-way quantum computing).

### Neutral-Atom Quantum Hardware:

* How is quantum information encoded in a neutral-atom qubit, i.e. what constitutes the two-level system with defined states  |0⟩  and  |1⟩?
  * Internal energy state of the atoms 

* How to initialize the neutral-atom qubit?
  * Using lasers to drive the atom to the desired initial state 
  
* How can we improve the coherence time of neutral-atom qubits?
  * Reducing external sources of noise, for example, laser phase noise 

* How can we implement gates using neutral-atom qubits? (Hint: in classical computing we switch between 0 and 1 in a controlled way)
  * Exciting the atoms from one internal energy state to another 
 
* Which fundamental atomic interaction is used to implement two qubit gates for neutral-atom quantum computing?
  * Dipole-Dipole interaction between Rydberg atoms 
  
* How do we differentiate between the qubit states for measurement?
  * Detecting light emitted from the atoms when probed with a laser beam 

* What are the most common sources of errors in neutral-atom quantum computing?
  * State preparation errors 
  * Dephasing of the Rydberg state 
  * State detection errors 

* What is a unique feature of quantum computers based on cold atoms?
  * They can perform digital and analog quantum computing.
 
* What are the main limitations in scaling neutral-atom quantum computers?
  * Laser power and uniform atomic array generation for large devices.

* State an advantage and a disadvantage of neutral atoms as a quantum computing platform. 
  * Advantages: They are all identical to one another and are simultaneously capable of storing and processing quantum information. This uniformity gives them an edge over manufactured qubits, which can suffer from imperfections.
  * Disadvantages: The gate operations are slower than in superconducting qubits. This is because physical qubit movement (qubit shuttling) is involved both in the initial setup of the system as well as in moving qubits near each other so that they can be entangled.

### Trapped-Ion Quantum Computing

* How is quantum information encoded in a trapped-ion qubit, i.e. what constitutes the two-level system with defined states |0⟩ and |1⟩? 
  * Information is encoded in internal states of each ion.

* How to initialize the trapped-ion qubit?
  * Lasers and in some instances microwave radiation is used to excite the population to an auxiliary state, after which it will decay to state |0⟩. 

* How can we improve the coherence time of trapped-ion qubits?
  * Increase the trapping potential amplitude to achieve better confinement of the qubit. 

* How can we implement gates using ions? (Hint: in classical computing we switch between 0 and 1 in a controlled way) 
  * We use resonant electromagnetic radiation to drive the ion between the |0⟩ and |1⟩ states. 

* Two qubit gates use ion entanglement. For this we need the ions to share a common interaction mode. Which is usually this “common mode” used to entangle ions in a trap?
  * The motional mode: the harmonic oscillator-like motion of multiple ions in the trap. 
  
* How do we differentiate between the qubit states for measurement?
  * Use laser light resonant with one of the states, which will fluoresce. If the ion doesn’t fluoresce, it is in the other state. 
  
* What are the most common sources of errors in trapped-ion quantum computing?
  * Electrical noise that can affect the ion motion in the trap and cause decoherence. 
  * Magnetic field noise that introduces a detuning in magnetic field sensitive states. 
  * Spontaneous scattering of laser light. 

* What are SPAM errors?
  * The errors associated with optical pumping and state-dependent fluorescence. 

* What are the consequences of Earnshaw’s theorem when it comes to designing ion traps?
  * The ion traps must use oscillating RF electric fields to confine the ions. 

* State an advantage and a disadvantage of trapped-ions as a quantum computing platform.
  * Advantage : Naturally lower error rates, with bias (easier to correct); First qubit technology (head start in R&D); all-to-all connectivity demonstrated in groups of tens of qubits.
  * Disadvantage : Hard to individually access each qubit (only done in linear arrays); Hard to trap many ions; Operations are relatively slow.

## Classiq - Quantum Algorithm Development. (Level 1)
Classiq Advanced Algorithms QC implementation. Minimal Circuit Depth, Circuit Optimization, Most Significant bit- Least significant bit exercises.

## Classiq - Quantum Algorithm Development. (Level 2)
Quantum Fourier Transform, Non unitary operations and Quantum Walk. Assignments are in jupyter notebook formats in the respective folder. A short summary is provided below against each.

## Pennylane - Quantum Machine Learning
Minimize the cost function (expval) with respect to test parameters for a custom variational circuit. Simple stuff. 

---

#### Project chosen for the Womanium cohort:- QML for Conspicutiy Detection (FRAUNHOFER)

Project specific `README.md` can be found in the respective directory.