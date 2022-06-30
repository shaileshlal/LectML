# Convolutional Neural Networks

The following notebooks are included:

1. [VisualizingFilters](VisualizingFilters.ipynb)

    Visualizing the effect of hand-tooled filters for edge detection on real world images.

2. [ConvNet_FashionMNIST](ConvNet_FashionMNIST.ipynb)

    Classifying the Fashion MNIST dataset using a convolutional network. The accuracy on the test set improves from 89% approx for MLPs to 92% here.

3. [VisualizeConvNet](VisualizeConvNet.ipynb)

    Visualizing what a Convolutional Neural Network learns by examining how its filters are activation.

4. [FullyConvNet_FashionMNIST](FullyConvNet_FashionMNIST.ipynb)

    Constructing a fully convolutional neural network, i.e. without any dense layers, to classify the Fashion MNIST dataset. The neural network is equivalent to [the previous one](ConvNet_FashionMNIST.ipynb) by design and reaches the same accuracy on the test set.

5. [ResNet20cifar10](Resnet20cifar10.ipynb)

    Classifying the CIFAR 10 dataset using a residual network and implementing the one-cycle learning rate. The analysis follows [this one](https://keras.io/zh/examples/cifar10_resnet/) where only the learning rate scheduling has been swapped out from an annealing schedule to the one cycle policy.
