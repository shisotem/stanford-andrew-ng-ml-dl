# Advice for applying machine learning

## Deciding what to try next

- This week, you'll learn a set of tips for determining **what to do next** in a machine learning project. This will enable you to use your time more efficiently.

  - Avoid spending a long time collecting data only to realize later that it was pointless.

  ![alt text](resources/notes/01.png)

  ![alt text](resources/notes/02.png)

## Evaluating a model

- We need a more systematic approach than just plotting f(x) to evaluate the performance of your model.

  - For only x<sub>1</sub> (single feature):

    - Fitting a fourth order polynomial to just five data points results in a very wiggly curve. From this, we can see that the generalization performance is low.

  - For x<sub>1</sub>, x<sub>2</sub>, x<sub>3</sub>, x<sub>4</sub> (multiple features):

    - Firstly, it's inherently challenging to plot a four-dimensional function f(x).

  ![alt text](resources/notes/03.png)

- Splitting the dataset into ratios such as 70-30 or 80-20.

  ![alt text](resources/notes/04.png)

  ![alt text](resources/notes/05.png)

## Model selection and training/cross validation/test sets

## Optional Lab: Model Evaluation and Selection
