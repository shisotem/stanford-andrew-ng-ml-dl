# Bias and variance

## Diagnosing bias and variance

- The **most powerful diagnostic** that I know of and have used for a lot of machine learning applications, is "bias and variance". This gives you very good guidance on **what to try next**.

- A systematic way to diagnose whether your algorithm has high bias or high variance, using **training and dev error** metrics (not depending on plotting):

  - **J<sub>train</sub> is high** &rarr; high bias

  - J<sub>train</sub> is low & J<sub>cv</sub> is also pretty low &rarr; just right!

  - **J<sub>cv</sub> >> J<sub>train</sub>** &rarr; high variance

  ![alt text](resources/notes/01.png)

- A different view on bias and variance:

  ![alt text](resources/notes/02.png)

  - **Most** learning applications have either high bias or high variance, **not both**. However, in some **neural network** applications, you might unfortunately encounter **both issues simultaneously**.

  ![alt text](resources/notes/03.png)

- When training machine learning algorithms, I almost always try to understand to what extent the algorithm has a problem with high bias (underfitting) or high variance (overfitting).

  - This provides good guidance on how to improve the performance of the algorithm, as we will see later this week.

## Regularization and bias/variance

- How can you choose a good value of &lambda;?

  ![alt text](resources/notes/04.png)

  - This procedure is similar to the procedure to choose d (degree of polynomial) using cross-validation.

  ![alt text](resources/notes/05.png)

  - Assess the cross-validation error for various &lambda;/d values, and choose the &lambda;/d that yields the lowest error for a hopefully good model.

  ![alt text](resources/notes/06.png)

## Establishing a baseline level of performance

- If even a human makes a 10.6% error, then it seems difficult to expect a learning algorithm to perform significantly better than it.

  - J<sub>train</sub>=10.8% means that your model accurately transcribes 89.2% of your training set, but makes errors in the remaining 10.8%.

  ![alt text](resources/notes/07.png)

- **Baseline level of performance** refers to the level of error that you can reasonably hope your learning algorithm to eventually achieve.

  ![alt text](resources/notes/08.png)

- (Note: There are occasional cases where the baseline level is 0%.)

  ![alt text](resources/notes/09.png)

## Learning curves

- Learning curves (For f<sub>w,b</sub>(x) = w<sub>1</sub>x + w<sub>2</sub>x<sup>2</sup> + b):

  - It may not be surprising that as the training set size gets bigger, the model improves and so the cross-validation error goes down.

  - The cross-validation error will typically be higher than the training error, as the parameters are fitted to the training set.

  ![alt text](resources/notes/10.png)

- High bias (f<sub>w,b</sub>(x) = w<sub>1</sub>x + b):

  - Given that this model is **too simple** (**high bias**), even if there is **more data**, both errors will just **plateau** and **J<sub>cv</sub> cannot approach the baseline level** of performance almost forever.

  ![alt text](resources/notes/11.png)

## Deciding what to try next revisited

## Bias/variance and neural networks

## Optional Lab: Diagnosing Bias and Variance
