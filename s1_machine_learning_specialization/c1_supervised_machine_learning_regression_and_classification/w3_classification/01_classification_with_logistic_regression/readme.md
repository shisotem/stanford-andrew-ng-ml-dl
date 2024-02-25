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

- Interpretation of logistic regression output:

  - **Probability** of **y=1** on input x

  ![alt text](resources/notes/05.png)

- Q:

  ![alt text](resources/questions/02.png)

- For a long time, many internet ads operated on a slightly modified version of logistic regression.

## Optional lab: Sigmoid function and logistic regression

## Decision boundary

## Optional lab: Decision boundary
