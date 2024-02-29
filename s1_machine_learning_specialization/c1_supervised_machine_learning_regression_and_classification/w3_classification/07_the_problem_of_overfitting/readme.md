# The problem of overfitting

## The problem of overfitting

- **Underfit** = **High bias** ↔ Just right &#9834; = Generalization ↔ **Overfit** = **High variance**

  - Underfitting: Caused by high bias (**preconception**), like assuming data is linear.

  - **Generalization**: Ability to predict accurately on unseen examples.

  - Overfitting: Occurs with **high-order polynomials** with **many features**.

    - Parameters make cost function zero (error is zero for all training examples).

    - **Works well on training set, but not on new examples**.

    - Slight changes in training set drastically alter the applied function.

  ![alt text](resources/notes/01.png)

  ![alt text](resources/notes/02.png)

- Q:

  ![alt text](resources/questions/01.png)

## Addressing overfitting

- We'll now learn to **address** overfitting. (Later in this specialization, we'll learn to **diagnose** it and underfitting.)

- If **more training data** is available, fitting a high order polynomial or feature-rich function can continue.

  - **This is ideal, if feasible**.

  ![alt text](resources/notes/03.png)

- **Feature selection**: Picking optimal features.

  - Reducing features, i.e., setting parameter w<sub>j</sub> to zero.

  - e.g.

    - [w<sub>1</sub>x + w<sub>2</sub>x<sup>2</sup> + w<sub>3</sub>x<sup>3</sup> + w<sub>4</sub>x<sup>4</sup> + b &rarr; w<sub>1</sub>x + w<sub>2</sub>x<sup>2</sup> + b](https://github.com/shisotem/stanford-andrew-ng-ml-dl/blob/main/s1_machine_learning_specialization/c1_supervised_machine_learning_regression_and_classification/w3_classification/07_the_problem_of_overfitting/resources/notes/01.png)
    - w<sub>1</sub>x<sub>1</sub> + w<sub>2</sub>x<sub>2</sub> + ... + w<sub>100</sub>x<sub>100</sub> + b &rarr; w<sub>1</sub>x<sub>1</sub> + w<sub>2</sub>x<sub>2</sub> + w<sub>4</sub>x<sub>4</sub> + b

  - Drawback: May lose useful prediction info.

  - (Algorithms for automatic feature selection come later in Course 2.)

  ![alt text](resources/notes/04.png)

- **Regularization**: Gently reduces some features' influence to prevent overfitting, without eliminating them.

  - Tips: Regularizing b is optional, but it makes little difference. **I usually don't**. Regularizing w<sub>1</sub> to w<sub>n</sub> is enough.

  - (Applicable to neural networks.)

  ![alt text](resources/notes/05.png)

- Just for myself, **I use regularization all the time**.

  ![alt text](resources/notes/06.png)

- Q:

  ![alt text](resources/questions/02.png)

## Optional lab: Overfitting

## Cost function with regularization

- a

  ![alt text](resources/notes/07.png)

  ![alt text](resources/notes/08.png)

  ![alt text](resources/notes/09.png)

- Q:

  ![alt text](resources/questions/03.png)

## Regularized linear regression

- a

- Q:

## Regularized logistic regression

- a

- Q:

## Optional lab: Regularization
