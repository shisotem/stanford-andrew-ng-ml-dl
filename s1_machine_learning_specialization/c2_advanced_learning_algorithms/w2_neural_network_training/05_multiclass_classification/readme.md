# Multiclass Classification

## Multiclass

- e.g. Classify pictures of pills into categories: scratch, discoloration, chip, etc.

  ![alt text](resources/notes/01.png)

  ![alt text](resources/notes/02.png)

## Softmax

- The **softmax regression** algorithm is a generalization of the logistic regression algorithm.

  - If you apply softmax regression with N equals 2, the parameters end up being a little bit different, but it ends up reducing to the logistic regression model.

  ![alt text](resources/notes/03.png)

- If y is equal to 2, the loss for this example is the negative log of the probability that y was predicted to be 2. (Note: we do not compute the negative log of a<sub>1</sub> or any other terms in this case.)

  - If y = j, the smaller a<sub>j</sub> is, the bigger the loss.

  ![alt text](resources/notes/04.png)

## Neural Network with Softmax output

- This neural network includes a **softmax activation function**, has a **softmax layer** as the output layer, and produces **softmax output**.

- Unique properties of a softmax activation function:

  - (sigmoid, ReLU, linear: a<sub>1</sub> is a function of z<sub>1</sub>)

  - softmax: a<sub>1</sub> is a function of z<sub>1</sub>, z<sub>2</sub>, ..., z<sub>N</sub>

  ![alt text](resources/notes/05.png)

- Specify the loss function in Step 2:

  - (For binary classification, use BinaryCrossentropy also known as logistic loss.)

  - For multiclass classification, use **SparseCategoricalCrossentropy**.

    - "Sparse" indicates that y can only take on one of these 10 values (0 ~ 9).

  ![alt text](resources/notes/06.png)

## Improved implementation of softmax

## Classification with multiple outputs (Optional)

## Softmax

## Multiclass
