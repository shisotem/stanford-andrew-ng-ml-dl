# TensorFlow implementation

## Inference in Code

- **TensorFlow** is one of the leading frameworks for implementing **deep learning** algorithms. (**PyTorch** is another one.)

- One of the remarkable things about **neural networks** is the **same algorithm** can be applied to so many **different applications**.

  ![alt text](resources/notes/01.png)

- The syntax for carrying out **inference** in TensorFlow:

  - "Dense" refers to a type of layer in the neural networks we've studied so far.

    - You'll learn about other types of layers later on.
    - For now, we'll stick with the **dense layer**.

  ![alt text](resources/notes/02.png)

  ![alt text](resources/notes/03.png)

  ![alt text](resources/notes/04.png)

- One more example:

  ![alt text](resources/notes/05.png)

- There are further details, like **loading the TensorFlow library and neural network parameters w and b**, not covered here. We'll address these in the lab, so please be sure to take a look.

## Data in TensorFlow

- How data is represented in NumPy and in TensorFlow:

  - NumPy was developed much earlier than TensorFlow.

  - Unfortunately, there are some inconsistencies between how data is represented in NumPy and in TensorFlow.

  ![alt text](resources/notes/06.png)

- 2D vs 1D:

  ![alt text](resources/notes/07.png)

- 2D array or 2D matrix where one of the dimensions happens to be 1.

  - TF, designed to handle very large datasets, uses 2D matrices instead of 1D vectors to improve computational efficiency.

- 1D array or 1D vector that has no rows or columns, just a list of numbers.

  - In linear regression or logistic regression, we use 1D vectors to represent the input features x.

  ![alt text](resources/notes/08.png)

## Building a neural network

## Coffee Roasting in Tensorflow
