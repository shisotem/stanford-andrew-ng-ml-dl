# Multiple linear regression

## Multiple features

- Review: Univariate Linear Regression

  ![alt text](resources/notes/01.png)

- Multiple Features & Notation

  ![alt text](resources/notes/02.png)

- Model of Multiple Linear Regression

  - **Multiple Linear Regression**: This is a type of linear regression that uses **multiple features**.

    - A model with **n features** can be represented as: f<sub>w,b</sub>(**x**) = w<sub>1</sub>**x<sub>1</sub>** + w<sub>2</sub>**x<sub>2</sub>** + ... + w<sub>n</sub>**x<sub>n</sub>** + b

  - Base Price: This refers to the starting price of a house, which is assumed to be $80,000, even if the house has no size, no bedrooms, no floors, and is not of any particular age.

  ![alt text](resources/notes/03.png)

  - (Note: The term "multivariate regression" refers to a different concept that we will not be using here.)

  ![alt text](resources/notes/04.png)

- Q:

  ![alt text](resources/questions/01.png)

- Next, we will discuss vectorization, which is necessary for implementing multiple linear regression.

## Vectorization part 1

- Learning how to write **vectorized** code will allow you to also take advantage of modern **numerical linear algebra libraries**, as well as possibly even **GPU** hardware.

- Two distinct benefits of vectorization:

  - It makes code **shorter**.

  - It also results in your code running much **faster** than non-vectorized implementations. This is because functions like NumPy's dot product can utilize **parallel hardware** in your computer, whether you're running this on a standard **CPU** or a **GPU**, which is often used to accelerate machine learning tasks.

  ![alt text](resources/notes/05.png)

- Q:

  ![alt text](resources/questions/02.png)

- Next, let's take a look at what your computer is actually doing behind the scenes to make vectorized code run so much faster.

## Vectorization part 2

- Use **Vectorization** in NumPy:

  - The dot function in NumPy is optimized for vectorization. It allows the computer to process all values of vectors w and x simultaneously, **multiplying corresponding pairs at the same time in parallel** (at t<sub>0</sub>).

  - Following this, the computer uses specialized hardware to **efficiently sum** these products, **eliminating the need for sequential additions** (at t<sub>1</sub>).

  - Consequently, vectorizing learning algorithms is a key step for efficient execution and scalability to large datasets.

  ![alt text](resources/notes/06.png)

## Optional lab: Python, NumPy and vectorization

## Gradient descent for multiple linear regression

## Optional Lab: Multiple linear regression
