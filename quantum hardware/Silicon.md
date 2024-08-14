### Silicon-based Quantum Hardware:

1. How is quantum information encoded in a silicon qubit, i.e. what constitutes the two-level system with defined states |0⟩ and |1⟩?
  * Information is encoded in the spin of the electron (residing in the potential well of a donor nucleus or quantum dot) or the spin of the donor nucleus 

2. How to initialize the silicon qubit?
  *  The electron is initialized by tuning the Fermi level of a single electron transistor to lie between the electron spin up and spin down energy levels . Only a spin down electron (|0⟩ state) will have enough energy to tunnel from the single electron transistor 

3. How can we improve the coherence time of silicon qubits?
  * Isotopically enrich the silicon to remove 29Si nuclear spins 
  * Increase the temperature of the dilution refrigerator to 1 K 
  * Increase the strength of the external magnetic field 

4. How can we implement gates using silicon qubits? (Hint: in classical computing we switch between 0 and 1 in a controlled way)
  * We use an on-chip microwave antenna to supply an oscillating magnetic field at a frequency resonant with the energy gap between the spin down and spin up states to drive between the |0⟩ and |1⟩ states.

5. Two qubit gates use entanglement. How can we entangle two spatially-separated donor spin qubits?
  *   Two flip flop qubits (created by the antiparallel spin states of a donor nucleus and electron) can be coupled by the electric dipole interaction when each electron is pulled away from its donor nucleus 
  * Two donor nuclear spins can be entangled through their hyperfine interaction with a shared electron spin 
  * Two electron spins can be entangled through the exchange interaction if the electron wavefunctions are close enough together to overlap with each other 

6. How do we differentiate between the qubit states for measurement?
  * A spin up electron (|1⟩ state) will tunnel onto a single electron transistor island causing the current flowing through the single electron transistor to change due to the altered charge environment. A spin down electron (|0⟩ state) will not have enough energy to tunnel onto the single electron transistor island, leaving the SET current unchanged .

7. What are the most common sources of errors in silicon-based quantum computing?
  * Electric field noise caused by two-level fluctuators in the environment (e.g charge traps at the oxide interface) result in decoherence 
  * Over or under-rotation of the quantum gates will introduce errors into your quantum circuit.
  * $^{29}Si$ nuclear spins in the environment decrease the coherence time of the electron spin by contributing to magnetic field noise. 

8. What is an advantage of using a heavier group V donor over the standard phosphorus donor?
  * Heavier donors have higher nuclear spin, providing a larger Hilbert space (with more energy levels) with the potential of encoding a qudit or multiple qubits 

9. How can spin qubits be fabricated in silicon?
  * Quantum dots can be defined by accumulating electrons under the oxide interface using on-chip electric gates, patterned using electron beam lithography 
  * Donor atoms can be placed inside the silicon crystal lattice using a scanning tunneling microscope lithography, phosphine dosing and silicon encapsulation. The donor provides both a nuclear and electron spin 
  * Donor atoms can be inserted into the silicon crystal lattice using ion implantation and annealing to repair the crystal. The donor provides both a nuclear and electron spin 

  (All of the above, depending on whether you want a donor spin qubit or just an electron spin qubit )

10. State an advantage and a disadvantage of silicon-based qubits as a quantum computing platform. 
  * Advantage: Smallest qubits (50 nm), so can fit a full useful quantum processor on a single chip; Qubits can be moved around; Can tolerate heating effects; Errors are easier to correct (biased errors).
  * Disadvantage: Small size requires state-of-the-art manufacturing partners; Tolerance to materials defects is low; requirement for advanced fabrication reflects in late onset for qubit count.