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

- Using the model f<sub>w,b</sub>(x) trained **only on the training set**, calculate **training error J<sub>train</sub>(w,b)** and **test error J<sub>test</sub>(w,b)**.

  ![alt text](resources/notes/05.png)

  - If J<sub>train</sub>(w,b) is low but J<sub>test</sub>(w,b) is high, it suggests the model performs well on the training set but fails to generalize to unseen data. &rarr; **Overfitting**

  ![alt text](resources/notes/06.png)

- In the context of applying machine learning to **classification problems**,

  ![alt text](resources/notes/07.png)

  - there's an alternative, and perhaps **more common**, definition of J<sub>test</sub>(w,b) and J<sub>train</sub>(w,b):

  - Rather than using logistic loss to compute test and training errors, it measures **the proportion of the test set and training set that the algorithm has misclassified**.

  ![alt text](resources/notes/08.png)

## Model selection and training/cross validation/test sets

- ([Generalization error](https://en.wikipedia.org/wiki/Generalization_error), also known as the out-of-sample error or the risk, is a measure of how accurately an algorithm is able to predict outcome values for previously **unseen data**.)

  ![alt text](resources/notes/09.png)

- Model selection on regression problems:

  - (d=1 denotes fitting a first-order polynomial.)

  - Flawed procedure:

    - (On the previous slide, we saw that if you were to fit w, b to the training data, then the training error J<sub>train</sub>(w,b) would be an overly optimistic estimate of the generalization error, meaning it's lower than the actual generalization error.)

    - Similarly, it turns out that if you choose the parameter d using the test set, the test error J<sub>test</sub>(w<sup><5></sup>,b<sup><5></sup>) becomes an overly optimistic estimate of the generalization error, meaning it's lower than the actual generalization error.

  ![alt text](resources/notes/10.png)

## Optional Lab: Model Evaluation and Selection
