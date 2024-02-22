# Gradient descent in practice

## Feature scaling part 1

- **Feature scaling** will enable gradient descent to run much **faster**.

- When a possible range of values of a **feature** is **large**, it's more likely that a good model will learn to choose a relatively **small parameter** value. Likewise, when the possible values of the **feature** are **small**, then a reasonable value for its **parameters** will be relatively **large**.

  ![alt text](resources/notes/01.png)

- A very **small change to w1** can have a very **large impact on the estimated price** and that's a very **large impact on the cost J**. In contrast, it takes a much **larger change in w2** in order to **change the predictions** much. And **small changes to w2**, **don't change the cost function** nearly as much.

  ![alt text](resources/notes/02.png)

- **Skinny** gradient descent may **oscillate** before finding the global minimum.

  - **Scaling features can help**, transforming data so that all features range from 0 to 1.

  - This allows for a more **direct path** to the global minimum.

  ![alt text](resources/notes/03.png)

- Recap: Features with different value ranges can **slow** gradient descent. **Rescaling to comparable ranges improves speed**.

## Feature scaling part 2

## Checking gradient descent for convergence

## Choosing the learning rate

## Optional Lab: Feature scaling and learning rate

## Feature engineering

## Polynomial regression

## Optional lab: Feature engineering and Polynomial regression

## Optional lab: Linear regression with scikit-learn
