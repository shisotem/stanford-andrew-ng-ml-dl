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
> Logistic regression: f<sub>w,b</sub>(x) = g(w&middot;x+b)
>
> - g(x) = 1 / (1 + e<sup>-x</sup>) &rarr; (same as sigmoid function)
>
> - g(2x) = 1 / (1 + e<sup>-2x</sup>) &rarr; shift x-axis by /2
>
> - g(x+2) = 1 / (1 + e<sup>-(x+2)</sup>) = g(x-(-2)) &rarr; shift x-axis by -2
>
> - g(2x+4) = 1 / (1 + e<sup>-(2x+4)</sup>) = g(2(x-(-2))) &rarr; shift x-axis by /2 and then -2
>
> - g(-0.5x+0.5) = 1 / (1 + e<sup>-(-0.5x+0.5)</sup>) = g(-0.5(x-1)) &rarr; shift x-axis by \*(-2) and then +1
>
> ![alt text](resources/notes/10.png)
>
> cf. What are the values of x to obtain the same output value of 1?
>
> - h(x) = x<sup>2</sup>
>
>   - **x = 1**
>
> - h(2x) = (2x)<sup>2</sup>
>
>   - 2x = 1
>   - &therefore; x = **1** /2 = 0.5
>   - i.e. shift x-axis by /2
>
> - h(x+2) = (x+2)<sup>2</sup> = h(x-(-2))
>
>   - x-(-2) = 1
>   - &therefore; x = **1** -2 = -1
>   - i.e. shift x-axis by -2
>
> - h(2x+4) = (2x+4)<sup>2</sup> = h(2(x-(-2)))
>
>   - 2(x-(-2)) = 1
>   - x-(-2) = 1 /2
>   - &therefore; x = **1** /2 -2 = -1.5
>   - i.e. shift x-axis by /2 and then -2
>
> - h(-0.5x+0.5) = (-0.5x+0.5)<sup>2</sup> = h(-0.5(x-1))
>
>   - -0.5(x-1) = 1
>   - x-1 = 1 /(-0.5)
>   - &therefore; x = **1** /(-0.5) +1 = **1** \*(-2) +1 = -1
>   - i.e. shift x-axis by \*(-2) and then +1
>
> ![alt text](resources/notes/11.png)

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
