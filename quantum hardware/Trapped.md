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