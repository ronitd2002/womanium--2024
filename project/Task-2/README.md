# Task 2

This tutorial intends to build a classifier for the Iris dataset. The initial steps are the same as implemented in the Parity Function python notebook. We import essential libraries along with the optimizer, set the device up, define a parametrized circuit, the variational classifier with bias added, the accuracy metric, and the cost function.

The crucial difference here, as compared to the Parity Function approximator, is that the Iris dataset has two continuous variables in the feature vector instead of binary inputs. Thus, a simple computational basis state vector preparation isn't helpful in this case.  

Instead, we decompose the feature vector, padded with two additional constant features, into angular rotations. These are further encoded as amplitudes in the state preparation using RY rotations and entanglement using CNOT gates.

We need to preprocess the data as follows:

Load the data. Pad the feature vector with constant values so as to match the dimension of the amplitude encoding, i.e., $2^2=4$. Normalize the inputs.

Now, we visualize the data - original, padded and normalized, and the angular encoding

We split the data randomly into 75:25 ratio for training and validation.

For the ansatz:

* We build a PQC.
* Initialize random weights. 
* Propose an ansatz: number of layers = 6

For the GDO, classical optimization : 

* Define the Nesterov Momentum Optimizer, which is a gradient-descent solver. 
* Set batch size = 5. 
* Train for sixty iterations, and monitor the cost and accuracy metrics for training and validation datasets. 

We want to obtain a balance in the training such that the model doesn't under/overfit the training data.

Now that the training is complete, we plot the data and decision boundary (contour)