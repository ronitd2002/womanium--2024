# Assignment 1

1. Code the algorithm of the Hadamard test that we covered in class using the Python SDK (below is a print screen of the Qmod for your convenience). 
2. Execute it from the SDK using 1,000 , 2,000 , 4,000 , 8,000 and 16,000 shots, and for each job calculate the (real part of the) expectation value using the formula $Re\{\bra{0}U_{QFT} \ket{0}\} = 2P_0 - 1$. 
3. Plot a graph of the expectation value as a function of the number of shots. Add the theoretical value to the graph. Explain the results. 

# Assignment 2

1. Apply the non-unitary matrix on a 1-qubit quantum state which has a 0.3 probability being measured in the zero state $\ket{0}$.
2. lcu operator matrix =>[[1,0],[0,0]]
3. breakdown sum = norm * (identity + Z)
init state = RY(theta = 2 * np.arccos(np.sqrt(0.3))) * $\ket{0}$

# Final Assignment - Classiq's Training

1. Follow the example from the 4th session for creating the quantum walk operator for the case of a circle with 4 nodes, and design the quantum walk operator for the case of a line with 16 nodes.
2. Create a well-detailed Python Jupyter notebook that explains your algorithm, including the code parts covered in class, and pictures/figures where relevant.
3. Utilize the attached Python code ([quantum_walk_circle_example.py](./quantum_walk_circle_example.py)) with the example from class for the task.
Feel free to extend the example beyond the requirements here and what was covered in class.
4. Contribute your notebook to the Classiq Git Library to the folder community/womanium/assignments.
5. Follow the [contribution guidelines](../../../CONTRIBUTING.md) in order to contribute - NO need to open an issue for this, you can directly open a PR
