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

- General case:

  - Model: f<sub>w,b</sub>(x) = wx + b

  - Parameters: w, b

  - Cost function: J(w, b) = (1 / 2m) \* Σ<sub>i=1</sub><sup>m</sup> (f<sub>w,b</sub>(x<sup>(i)</sup>) - y<sup>(i)</sup>)<sup>2</sup>

  - Goal: **minimize<sub>w, b</sub> J(w, b)**

    - Find the values of w, and b that minimize the cost function (to get the best fit line)

- Simplified case (b = ø):

  - f<sub>w</sub>(x) = wx

  - w

  - J(**w**) = (1 / 2m) \* Σ<sub>i=1</sub><sup>m</sup> (f<sub>**w**</sub>(x<sup>(i)</sup>) - y<sup>(i)</sup>)<sup>2</sup>

    - (= (1 / 2m) \* Σ<sub>i=1</sub><sup>m</sup> (**w**x<sup>(i)</sup> - y<sup>(i)</sup>)<sup>2</sup>)

  - minimize<sub>w</sub> J(w)

  ![alt text](resources/notes/05.jpg)

- Relationship between w, f<sub>w</sub>(x), and J(w):

  - Choosing a value for the parameter **w** specifies **a line function f(x)** on the left graph and **a single point** on the right graph.

  ![alt text](resources/notes/06.jpg)

- Q:

  ![alt text](resources/questions/03.png)

## Visualizing the cost function

- General case:

  - Model: f<sub>w,b</sub>(x) = wx + b

  - Parameters: w, b

  - Cost function: J(w, b) = (1 / 2m) \* Σ<sub>i=1</sub><sup>m</sup> (f<sub>w,b</sub>(x<sup>(i)</sup>) - y<sup>(i)</sup>)<sup>2</sup>

  - Goal: minimize<sub>w, b</sub> J(w, b)

- Relationship between w, b, f<sub>w,b</sub>(x) and J(w, b):

  ![alt text](resources/notes/07.jpg)

## Visualization examples

- minimize<sub>w, b</sub> J(w, b):

  ![alt text](resources/notes/08.jpg)

- In linear regression, manually reading a contour plot to find the best values for parameters **w** and **b** is not efficient or scalable for complex machine learning models. Instead, an algorithmic approach, such as **gradient descent**, is preferred for automatically finding these values that **minimize** the cost function **J**. Gradient descent is a crucial algorithm in machine learning.

## Optional lab: Cost function
