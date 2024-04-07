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

  - [Previous slide] Fit parameters w, b using the training set &rarr; The trained model is biased towards the training set &rarr; J<sub>train</sub>(w,b) < generalization error

  - [Current slide] Select parameter d (degree of polynomial) using the test set &rarr; The chosen model is biased towards the test set &rarr; J<sub>test</sub>(w<sup><5></sup>,b<sup><5></sup>) < generalization error

  - Flawed procedure:

    - (d=1 denotes fitting a first-order polynomial.)

  ![alt text](resources/notes/10.png)

  - Correct procedure:

    - Since **no decisions were made using the test set**, J<sub>test</sub>(w<sup><4></sup>,b<sup><4></sup>) will be a fair estimate of the generalization error of this model.

  ![alt text](resources/notes/11.png)

  ![alt text](resources/notes/12.png)

  ![alt text](resources/notes/13.png)

- Applicable to other types of models such as neural networks:

  - (Note: Since this is a **classification problem** - handwritten digit recognition - the most common approach to compute J<sub>cv</sub> is to consider it as the **fraction** of cross-validation examples that the algorithm has **misclassified**.)

  ![alt text](resources/notes/14.png)

- While making decisions about the learning algorithm (like fitting parameters or choosing a model architecture), it's **best practice** to only use the training set and cross-validation set, and **not look at the test set at all**.

## Optional Lab: Model Evaluation and Selection
