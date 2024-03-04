# Classification with logistic regression

## Motivations

- The assignment of true/1 or false/0 is often arbitrary. Often either choice could work. (e.g. non-spam: true/1, spam: false/0)

  ![alt text](resources/notes/01.png)

- What happens when you try to use linear regression for classification? - Often it will **not** work well.

  - For this particular training set, the blue line seems reasonable at first glance.
  - However, just by adding one training example to the right, the linear regression line (and decision boundary) shifts significantly to the right, resulting in a drastic decrease in prediction accuracy.

  ![alt text](resources/notes/02.png)

- Q:

  ![alt text](resources/questions/01.png)

## Optional lab: Classification

## Logistic regression

- **Logistic regression** is probably the single most widely used classification algorithm in the world.

  ![alt text](resources/notes/03.png)

  ![alt text](resources/notes/04.png)

- Interpretation of logistic regression output: **Probability** of **y=1** on input x

  ![alt text](resources/notes/05.png)

- Q:

  ![alt text](resources/questions/02.png)

- For a long time, many internet ads operated on a slightly modified version of logistic regression.

> [!NOTE]
>
> g(z) = 1 / (1 + e<sup>-z</sup>)
>
> g(z+4) = 1 / (1 + e<sup>-(z+4)</sup>) = g(z-(-4))
>
> g(2z+8) = 1 / (1 + e<sup>-(2z+8)</sup>) = g(2(z-(-4)))
>
> g(-0.5z+1) = 1 / (1 + e<sup>-(-0.5z+1)</sup>) = g(-0.5(z-2))
>
> ![alt text](resources/notes/10.png)

## Optional lab: Sigmoid function and logistic regression

## Decision boundary

- When does the prediction yield 1, and when does it yield 0?

  ![alt text](resources/notes/06.png)

- **Decision boundary**: If the threshold is 0.5, the decision boundary is **z=0**.

  - For instance, if the parameters are w<sub>1</sub>=1, w<sub>2</sub>=1, b=-3, the decision boundary is the following purple line:

  ![alt text](resources/notes/07.png)

  - You can use **polynomial features** to get more **complex** decision boundaries.

  ![alt text](resources/notes/08.png)

  ![alt text](resources/notes/09.png)

- Q:

  ![alt text](resources/questions/03.png)

## Optional lab: Decision boundary
