# Exercise 1

Follow: [Design (The QMod Language)](https://nightly.docs.classiq.io/latest/classiq_101/classiq_concepts/design/)

Task: Write within the IDE with the native syntax a quantum algorithm that coherently calculates $y= 2x + 4z +2$, where `x` and `z` are quantum numbers represented with 5 qubits each, and they are initialized in a superposition of all possible values.

# Exercise 2

Follow: [Design - Quantum Variables and Functions](https://nightly.docs.classiq.io/latest/classiq_101/classiq_concepts/design/quantum_variables_and_functions/)

Task: Create another quantum function `flip_lsb` that flips the least significant bit.

# Exercise 3

Follow: [Optimize - The Synthesis Engine tutoria](https://nightly.docs.classiq.io/latest/classiq_101/classiq_concepts/optimize/)

Task: Modify the constraints such that you optimize the circuit for minimal circuit depth using maximum 25 qubits. What are the circuit depth and width you receive? Are they different from the given example?

# Exercise 4

Follow: Open the example from the [Analyze - Classiq Visualization Tool](https://nightly.docs.classiq.io/latest/classiq_101/classiq_concepts/analyze/) tutorial.

Task: Export it as a LaTeX file, and view it in a LaTeX Editor (it is recommended to use Overleaf)

# Exercise 5

Follow: Follow the [Execute](https://nightly.docs.classiq.io/latest/classiq_101/classiq_concepts/execute/) tutorial.

Task A: Adapt the code such that the quantum number x is allocated with 10 qubits. 
Task B: Execute the algorithm with 5096 shots and post process the results from your Python SDK. Plot a graph of all the measured values of `x` and `y` with the corresponding axes (make sure you receive the graph of $y=x^2 +1$).

# **Assignment 1**

Implement a Multi-Control-X

**Task A:** 
1. Synthesize 3 different implementations of an MCX (multi-control-x) with 5 control qubits and 1 target qubit (you should use the `control` quantum operation for implementing an MCX, follow [this](https://docs.classiq.io/latest/explore/functions/function_usage_examples/mcx/mcx_example/). tutorial that can be open in the IDE).
2. One implementation should be optimized for minimized depth, the other for minimized width, and the third somewhere in between (choose yourself what is the maximal width / depth you apply).
3. Export the 3 implementations as LaTeX files on the hierarchy level that demonstrates the differences between the implementations. Aggregate the implementations in 1 file and export it as a PDF and explain the key differences. (It is recommended to use *Overleaf*. -  a free, easy to use online LaTeX editor)

**Task B:** 
1. Synthesize 2 different implementations of an MCX (multi-control-x) with 20 control qubits and 1 target qubit. 
2. Compare the circuit width and circuit depth required for each implementation.

### Submission guidelines
Deliverable: 1 PDF file with:
1. The three different circuit implementations of Task A with a brief explanation
2. The details of the two different implementations of Task B