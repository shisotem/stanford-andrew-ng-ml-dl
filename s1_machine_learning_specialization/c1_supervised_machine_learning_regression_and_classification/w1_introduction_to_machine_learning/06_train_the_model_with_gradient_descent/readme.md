# Train the model with gradient descent

## Gradient descent

- Gradient descent is a **crucial** algorithm not only in linear regression, but also across **all areas of machine learning** (including deep learning).

- Gradient descent is an optimization algorithm that you can use to try to **minimize any function**, not just a cost function for linear regression.

  - min<sub>w<sub>1</sub>,...,w<sub>n</sub>,b</sub> J(w<sub>1</sub>,...,w<sub>n</sub>,b)

- Gradient descent:

  - Situation:

    - Have some function J(w, b)
    - Want min<sub>w, b</sub> J(w, b)

  - Outline:

    - Start with some w, b (e.g. set w=0, b=0) &larr; initial guesses
    - Keep changing w, b to reduce J(w, b) until we settle at or near a minimum

- Note:

  ![alt text](resources/notes/01.jpg)

## Implementing gradient descent

- **Gradient descent algorithm**:

  - **Learning rate**: Controls the **step size** during each iteration of gradient descent.

  - **Derivative**: Indicates the **direction** of the steepest ascent. Gradient descent moves in the opposite direction, i.e., the direction of the steepest descent.

  - In locations where the gradient (dJ(w) / dw) is large, the parameter update size (α \* dJ(w) / dw) is also large.

  - Convergence refers to reaching a **local minimum** where parameters w and b barely change with additional steps taken.

  ![alt text](resources/notes/02.jpg)

- Q:

  ![alt text](resources/questions/01.png)

## Gradient descent intuition

- Simplified case(b = ø or fixed):

  - J(w)

  - w = w - &alpha; \* dJ(w) / dw

  - min<sub>w</sub> J(w)

  ![alt text](resources/notes/03.jpg)

  ![alt text](resources/notes/05.jpg)

- Q:

  ![alt text](resources/questions/02.png)

## Learning rate

- w = w - &alpha; \* dJ(w) / dw

  - If &alpha; is too **small**, gradient descent may be **slow**.

  - If &alpha; is too **large**, gradient descent may:
    - **Overshoot**, never reach minimum
    - Fail to converge, **diverge**

  ![alt text](resources/notes/04.jpg)

- Can reach local minimum without decreasing learning rate &alpha;.

  - Near a local minimum,

    - **Derivative** becomes smaller
    - **Update steps** become smaller

  ![alt text](resources/notes/06.jpg)

## Gradient descent for linear regression

- Gradient descent for linear regression:

  ![alt text](resources/notes/07.jpg)

  ![alt text](resources/notes/08.jpg)

## Running gradient descent

## Optional lab: Gradient descent
