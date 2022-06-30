# Neural Networks

These notebooks provide some computations using Keras for neural networks arranged in somewhat increasing degrees of sophistication, starting with an out-of-the box application. The other notebooks demonstrate additional ways in which one can control the training of a neural network first through [callbacks](https://keras.io/api/callbacks/) and secondly through designing the training loop from the ground up.

1. [BaseMLP](BaseMLP.ipynb)

Introduces Keras by building a simple artificial neural network to classify the FMNIST dataset. We use the standard <tt>model.fit</tt> idiom to fit data to the neural network, and evaluate the performance of the model on a holdout test set. We also analyze misclassifications for some isolated cases and find that they are largely plausible, i.e. a shoe has been mistaken for a sneaker or a shirt for a t-shirt and so on.

2. [LRCallbacks](LRCallbacks.ipynb)

Utilizes callbacks to implement [Leslie Smith's strategies](https://arxiv.org/abs/1803.09820) for determining the optimal learning rate.

3. [MonitorGradients](MonitorGradients.ipynb)

Tests Glorot and He initialization to verify that these do indeed alleviate the problem of vanishing gradients. Instead of using the <tt>model.fit</tt> idiom, we design a custom training loop for a single epoch, i.e. about a thousand iterations of gradient descent. The custom loop follows the tutorial [here](https://keras.io/guides/writing_a_training_loop_from_scratch/).
