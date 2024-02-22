# Gradient descent in practice

## Feature scaling part 1

- When a possible range of values of a feature is large, it's more likely that a good model will learn to choose a relatively small parameter value. Likewise, when the possible values of the feature are small, then a reasonable value for its parameters will be relatively large.

  ![alt text](resources/notes/01.png)

- A very small change to w1 can have a very large impact on the estimated price and that's a very large impact on the cost J. In contrast, it takes a much larger change in w2 in order to change the predictions much. And small changes to w2, don't change the cost function nearly as much.

  ![alt text](resources/notes/02.png)

> [!IMPORTANT]
>
> The key points of this lecture are:
>
> When **features** have **different ranges** as in the top-left graph, the **cost function** becomes **skinny** as in the top-right graph, **slowing** the learning. In such cases, it's crucial to **scale features to comparable ranges** as in the bottom-left graph. This results in a **circular cost function** as in the bottom-right graph, **speeding up** the learning.
>
> ![alt text](resources/notes/03.png)

## Feature scaling part 2

- a

  ![alt text](resources/notes/04.png)

  ![alt text](resources/notes/05.png)

  ![alt text](resources/notes/06.png)

  ![alt text](resources/notes/07.png)

- Q:

  ![alt text](resources/questions/01.png)

## Checking gradient descent for convergence

- a

  ![alt text](resources/notes/08.png)
  ｆ
  ![alt text](resources/notes/09.png)

## Choosing the learning rate

- a

  ![alt text](resources/notes/10.png)

  ![alt text](resources/notes/11.png)

- Q:

  ![alt text](resources/questions/02.png)

## Optional Lab: Feature scaling and learning rate

## Feature engineering

- a

  ![alt text](resources/notes/12.png)

- Q:

  ![alt text](resources/questions/03.png)

## Polynomial regression

- a

  ![alt text](resources/notes/13.png)

  ![alt text](resources/notes/14.png)

## Optional lab: Feature engineering and Polynomial regression

## Optional lab: Linear regression with scikit-learn
