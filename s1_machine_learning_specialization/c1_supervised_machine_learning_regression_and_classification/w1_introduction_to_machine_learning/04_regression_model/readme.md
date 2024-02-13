# Regression Model

## Linear regression model part 1

- Terminology & Notation:

  - **Training set**: Data used to train the model

  - x = "input" variable / feature
  - y = "output" variable / "target" variable
  - m = number of training examples
  - (x, y) = single training example
  - (x<sup>(i)</sup>, y<sup>(i)</sup>) = i<sup>th</sup> training example

- e.g.:

  ![alt text](resources/notes/01.jpg)

  - x<sup>(1)</sup> = 2502
  - y<sup>(1)</sup> = 280

  - m = 18

  - (x<sup>(1)</sup>, y<sup>(1)</sup>) = (2502, 280)
  - x<sup>(2)</sup> = 1010
    - x<sup>(2)</sup> ≠ x<sup>2</sup> ... not exponent!

## Linear regression model part 2

- The process of how supervised learning works:

  ![alt text](resources/notes/02.jpg)

- Q:

  ![alt text](resources/questions/01.png)

## Optional lab: Model representation

## Cost function formula

- Model: **f<sub>w,b</sub>**(x) = **w**x + **b**

  - **w, b**: **parameters** (coefficients, weights)

  ![alt text](resources/notes/03.jpg)

- Cost function: **J(w, b)**

  - **1 / m**: To build a cost function that doesn't automatically get bigger as the training set size gets larger (by convention)

  - The extra division by **2** is just meant to make some of our later calculations **look neater**.

  - Eventually we're going to want to find values of **w** and **b** that make the **cost function small**.

  ![alt text](resources/notes/04.jpg)

- Q:

  ![alt text](resources/questions/02.png)

## Cost function intuition

## Visualizing the cost function

## Visualization examples

## Optional lab: Cost function
