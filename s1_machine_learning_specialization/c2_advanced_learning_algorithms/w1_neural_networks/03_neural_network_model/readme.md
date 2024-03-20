# Neural network model

## Neural network layer

- How to construct a "layer" of neurons:

  - These four numbers are inputs to **each** of three neurons.

  - There's a 0.3 chance of this being highly affordable based on the input features.

  - Remember whenever you see "<sup>**[1]**</sup>", that just refers to a quantity that is **associated with layer 1** of the neural network.

    - e.g. **w**<sub>2</sub><sup>[1]</sup>, b<sub>2</sub><sup>[1]</sup> are the parameters of the second hidden unit or the second hidden neuron in layer 1.

  ![alt text](resources/notes/01.png)

- In this example, because the **output layer has just a single neuron**, the **output is a scalar**, which is a single number rather than a vector of numbers.

  ![alt text](resources/notes/02.png)

- Optional final step: Is this a top seller? (Yes/No, not probability)

  ![alt text](resources/notes/03.png)

## More complex neural networks

- By convention, when we say a neural network has four layers, this includes all the hidden layers and the output layer, but not the input layer.

  ![alt text](resources/notes/04.png)

- Reconfirm:

  ![alt text](resources/notes/05.png)

  ![alt text](resources/notes/06.png)

- General equation:

  ![alt text](resources/notes/07.png)

## Inference: making predictions (forward propagation)

- This is just a binary classification problem where we input an image and classify it as either the digit zero or one.

  ![alt text](resources/notes/08.png)

  ![alt text](resources/notes/09.png)

- You can also write the output of the neural network as **f(x)**.

  - Remember that we use f(x) to denote the output of linear regression and logistic regression.

- This is neural network **inference** via **forward propagation**.

  - It propagates neuron activations from left to right.

  - It is in contrast to the **learning algorithm**, **back propagation**.

  - (With this, you can download parameters from an online pre-trained neural network and make inferences on your new data.)

- This is a neural network architecture, which starts with more hidden units that decrease towards the output layer. There's also a pretty typical choice when choosing neural network architectures. (&rarr; more examples in the lab)

  ![alt text](resources/notes/10.png)

## Neurons and Layers
