# Bias and variance

## Diagnosing bias and variance

- The **most powerful diagnostic** that I know of and have used for a lot of machine learning applications, is "bias and variance". This gives you very good guidance on **what to try next**.

- A systematic way to diagnose whether your algorithm has high bias or high variance, using **training and dev error** metrics (not depending on plotting):

  - J<sub>train</sub> is high &rarr; high bias

  - J<sub>train</sub> is low & J<sub>cv</sub> is also pretty low &rarr; just right!

  - J<sub>cv</sub> >> J<sub>train</sub> &rarr; high variance

  ![alt text](resources/notes/01.png)

- A different view on bias and variance:

  ![alt text](resources/notes/02.png)

## Regularization and bias/variance

## Establishing a baseline level of performance

## Learning curves

## Deciding what to try next revisited

## Bias/variance and neural networks

## Optional Lab: Diagnosing Bias and Variance
