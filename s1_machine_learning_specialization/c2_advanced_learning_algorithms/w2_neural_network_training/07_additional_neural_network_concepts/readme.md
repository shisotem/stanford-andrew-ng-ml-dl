# Additional Neural Network Concepts

## Advanced Optimization

- **Adam**, an optimization algorithm faster than gradient descent, is the **de facto standard** for practitioners training neural networks.

  - It **adjusts the learning rate automatically**.

  ![alt text](resources/notes/01.png)

  - It uses **different learning rates for each parameter**.

  ![alt text](resources/notes/02.png)

  - Details on Adam's automatic learning rate adjustment aren't covered in this course. (&rarr; Learn more about Adam in the DL Specialization)

  ![alt text](resources/notes/03.png)

- How you implement Adam:

  - Adam requires an initial learning rate, like 10<sup>-3</sup>. It's more **robust** to your initial learning rate choice than gradient descent as it can slightly adjust the learning rate automatically. Still, it's **beneficial to try a few values** for this default global learning rate, to somewhat speed up the learning.

  ![alt text](resources/notes/04.png)

## Additional Layer Types

- Each neuron in the **dense** layer takes inputs from **all** neurons in the previous layer.

  ![alt text](resources/notes/05.png)

- Each neuron in the **convolutional** layer takes inputs from **only a subset** of neurons (commonly limited **little square** regions of the input image) in the previous layer.

  ![alt text](resources/notes/06.png)

- **Convolutional Neural Network** (**CNN**) using 1D EKG signals (ElectroCardioGrams), not 2D images as input data:

  ![alt text](resources/notes/07.png)
