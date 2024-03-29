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

- The computer has only a **finite** amount of memory to store each number, a floating-point number in this case. Therefore, depending on **how we compute** the value 2/10000, the result can have more or less numerical **round-off error**.

  ![alt text](resources/notes/07.png)

  ![alt text](resources/notes/08.png)

- There's an alternative method to formulate the loss function for softmax. This method helps **reduce round-off errors**, resulting in more precise calculations in TensorFlow.

- First explanation using logistic regression:

  - Tell TensorFlow to compute 'a' as an **intermediate** term (This is also a model's final output). Then, compute the loss using **precalculated** 'a'. This is like (1 + 1/10000) - (1 - 1/10000), where (1 + 1/10000) and (1 - 1/10000) are intermediate terms.

  - For logistic regression, this implementation works okay, and usually the numerical round-off errors aren't that bad.

  ![alt text](resources/notes/09.png)

  - However, to prevent TensorFlow from computing 'a' as an intermediate term, I expanded 'a' directly into the loss function. This allows TensorFlow to freely rearrange the terms within the loss function, to compute the loss in a more numerically accurate way. This is like 2/10000.

  ![alt text](resources/notes/10.png)

- Softmax regression:

  ![alt text](resources/notes/11.png)

  ![alt text](resources/notes/12.png)

- More details:

  ![alt text](resources/notes/13.png)

  ![alt text](resources/notes/14.png)

## Classification with multiple outputs (Optional)

## Softmax

## Multiclass
