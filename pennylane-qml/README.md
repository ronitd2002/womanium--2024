# QML Challenge - Pennylane

## Challenge Statement

In this challenge, you will be provided with a variational quantum circuit in PennyLane that depends on a set of trainable parameters. The circuit outputs a single number as the expectation value of a fixed measurement. Your objective is to find the minimum expectation value this circuit can produce by optimizing its parameters. This will require converting the circuit into a QNode. You can either code up your own optimizer by calculating the gradient of the QNode, or you can use one of the provided PennyLane optimizers.

## Challenge code

The `variational_circuit` function contains the quantum circuit and has a `params` argument for specifying the trainable parameters. These are the parameters that need to be updated by the optimizer. Additionally, it has a `hamiltonian` argument, which specifies an unknown Hamiltonian that is used as an observable. The parameters describing the Hamiltonian are not trainable!

You must fill in the `optimize_circuit` function so that it minimizes the variational circuit. The trainable input to this function is a `params` argument that specifies the initial parameters to use when optimizing the `variational circuit`. The `hamiltonian` argument is the same as for `variational_circuit`, and is needed here since you are expected to call `variational_circuit` within this function. In `optimize_circuit`, you will need to convert the variational circuit into an executable QNode using `qml.QNode()`.

In both functions, the Hamiltonian is specified by the problem input data, with each Hamiltonian resulting in a different minimum for the variational circuit.

## Input
As input to this problem, you are given `hamiltonian` (`np.array(float)`), which is a list of parameters that encode the secret Hamiltonian whose expectation value is to be minimized.

## Output
The code will output a `float` corresponding to the minimum expectation value of the secret Hamiltonian, found by optimizing the input parameters in `variational_circuit`.