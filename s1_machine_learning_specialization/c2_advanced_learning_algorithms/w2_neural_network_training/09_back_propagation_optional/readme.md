# Back Propagation (Optional)

## What is a derivative? (Optional)

> [!IMPORTANT]
>
> In TensorFlow, you specify a neural network architecture, f<sub>W,B</sub>(x), and a loss function, L(f<sub>W,B</sub>(x),y). Adam then trains the network parameters using the **derivatives computed by back propagation**.

- ∂J(w)/∂w = 6: **"If w goes up by a tiny little amount ε, J(w) goes up 6 times as much."**

  ![alt text](resources/notes/01.png)

  ![alt text](resources/notes/02.png)

  ![alt text](resources/notes/03.png)

- Derivative examples:

  ![alt text](resources/notes/04.png)

  ![alt text](resources/notes/05.png)

  ![alt text](resources/notes/06.png)

- Notation:

  ![alt text](resources/notes/07.png)

## Computation graph (Optional)

- Forward prop:

  ![alt text](resources/notes/08.png)

- **Forward prop &rarr; (remember w, c, b, a, d, J) &rarr; Back prop**:

  - For example, if d increases from 2 to 2.001 (+0.001), then J increases from 2 to 2.0020005 (+0.002). Therefore, **∂J/∂d** = 2.

  - **Chain rule**: ∂J/∂w = (((**∂J/∂d**) \* ∂d/∂a) \* ∂a/∂c) \* ∂c/∂w

  ![alt text](resources/notes/09.png)

  - Manually verify that ∂J/∂w equals -4:

  ![alt text](resources/notes/10.png)

- The efficiency of backprop:

  ![alt text](resources/notes/11.png)

> [!NOTE]
>
> - 🤯 Numerical Differentiation: ∂J(w)/∂w = (J(w+ε) - J(w-ε)) / 2ε. For example, as ε=1<sup>-4</sup>.
>
> - 🤯 Symbolic Differentiation: both the input and output are **expressions**, not values. For instance, the derivative of x<sup>2</sup> with respect to x is 2x.
>
> - 😎 **Automatic Differentiation** (Back Propagation): use the **chain rule** to compute both derivatives **efficiently** and **accurately**.

## Larger neural network example (Optional)

- asdf

  ![alt text](resources/notes/12.png)

  ![alt text](resources/notes/13.png)

  ![alt text](resources/notes/14.png)

## Optional Lab: Derivatives

## Optional Lab: Back propagation
