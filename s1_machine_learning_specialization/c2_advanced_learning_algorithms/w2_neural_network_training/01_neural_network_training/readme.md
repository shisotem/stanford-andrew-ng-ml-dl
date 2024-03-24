# Neural Network Training

## TensorFlow implementation

- "Train" a neural network in TensorFlow (in 3 steps):

  - `epochs=100` means the **entire** training set is passed through the neural network 100 times.

  ![alt text](resources/notes/01.png)

## Training Details

- Let's recall how you trained a logistic regression model:

  ![alt text](resources/notes/02.png)

- Details of training a neural network:

  ![alt text](resources/notes/03.png)

  - `tensorflow.keras`: This is the **Keras** library, which was originally developed independently, but eventually got merged into the TensorFlow framework.

  ![alt text](resources/notes/04.png)

  - Actually, TensorFlow can use an **optimization algorithm** faster than gradient descent (e.g., **Adam**), which you'll learn more about later this week.

  ![alt text](resources/notes/05.png)

- As libraries mature, most engineers prefer using them over implementing code from scratch.

  ![alt text](resources/notes/06.png)
