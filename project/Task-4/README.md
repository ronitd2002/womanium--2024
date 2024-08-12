## Task 4

The objective of this subtask was to develop a quantum model capable of learning the sine function over the interval $[0, 2\pi]$. We approached this by discretizing the interval into a suitable number of points and using the corresponding sine values at these points as labels. The goal was to implement a Quantum Machine Learning (QML) model that could approximate the sine function.

### Our approach

We set a cost function using a square loss error function. We used a PQC for the ansatz and trained it to fit the sine function which was discretized into 100 discrete intervals and appropriately split into testing and training datasets. We learn these parameters along with the classical "bias" parameter during the training phase.

Additionally, we also implement a **Classical Neural Network** to approximate the same function and analyze how it compares with the QML model and demonstrate the improvement and the advantage the quantum neural network model proves in this case.

### Strategy:

- **Input Encoding:**  
  We employed angle encoding to convert the input values (x-coordinates) into quantum states. This involved setting the angle of a rotation gate according to the input value.

- **Measurement:**  
  The output of the circuit was measured to generate predictions for sin(x). This was achieved by measuring the expectation value of a Pauli-Z operator on a specific qubit.

- **Cost Function Definition:**  
  To evaluate the model’s performance, we defined a cost function that measured the difference between the model’s predictions and the actual sine values. We opted for the Mean Squared Error (MSE)/ the Square loss as the cost function.

- **Optimization:**  
  The parameters of the quantum circuit were optimized using a classical optimization algorithm, such as gradient descent, to minimize the cost function.

- **Training:**  
  The optimization process was run on the training data, allowing the quantum model to learn the sine function.

- **Evaluation:**  
  After training, the model was tested on new points within the $[0, 2\pi]$ interval to assess its ability to approximate the sine function accurately.

  ## Classical Neural Network

  We implement a classical Neural Network made up of three hidden layers to approximate the sine function. The purpose is to compare it with the QML version of the same approximator.

  Discretize the interval of $[0, 2\pi]$ into a thousand points. Distribute them radomly into training and test datasets in 80:20 ratio. We use the test dataset to validate our trained model, to make sure it hasn't under/overfit the training data.

  After testing a few configurations of layers and number of neurons in each layer of the NN, we figured a configuration that works well in approximating the sine function. That is, we start with the input $x$, feed it to a hidden layer of 128 neurons. The next hidden layer is made up of 256 neurons, and the third one is made up of 128 again. 

Each layer is succeeded by a ReLU activation function. This provides the non-linearity to the network. The layer after is the output. Since the ReLU acitvation function has an output range of $[0, \infty]$, we also add an operation of $z = 2z-1$ at the end.

At the beginning of the operations in the network, we also divide the input by $\pi$ and subtract 1 from it to normalize the inputs into the interval of $[-1,1]$.

We use the inbuit MSELoss, i.e., Mean Squared Error Loss, provided by PyTorch, as the loss criterion. We also use a scheduler that drops the Learning Rate (LR) by a factor at a defined number of steps. This is for better approach to optimization, so that the Gradient Descent algorithm doesn't get stuck oscillating around a local optima due to a relatively larger LR when it could go to a better approximation of the local optima with a lower LR.

Post-training, we check how the approximation is for a random number in the interval. After that we compute the trained model's approximations for both train and test datasets, and plot them.

# Results, comparisons and Quantum Advantage
The results are attached below for both the classical and quantum training and it's glaringly obvious that the quantum method clearly outperforms the classical implementation.

![classical results](https://github.com/shreyas-p56/QML-for-Conspicuity-Detection-in-Production/blob/main/Task-4/classical-pred.png?raw=true)

![quantum results](https://github.com/shreyas-p56/QML-for-Conspicuity-Detection-in-Production/blob/main/Task-4/quantum-pred.png?raw=true)

The first plot corresponds to the classical implementation while the second one corresponds to quantum implementation.