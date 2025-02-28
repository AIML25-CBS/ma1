**AI & Machine Learning (KAN-CINTO4003U) - Copenhagen Business School | Fall 2025**

***

### Group members
| Student name | Student ID |
| --- | --- |
| Emil Stausbøl | 152025 |
| Simon Hjorth Jensen | 153308 |


***

<br>

# Mandatory assignment 1

This repository contains the first mandatory assignment (MA1) for AIML25. It consists of two parts: Artificial Neural Networks and Convolutional Neural Networks. Please read the description for each part of the assignment carefully. 

* **Dev setup**: To complete this assignment, you will need to have followed the Development Setup guide. Please complete this setup before starting the assignment.

* **Helper code**: You are given a lot of boilerplate code as functions in `/src` to be imported into each of the notebooks. This is to simplify the assignments. Please acquaint yourself with this "helper code".

* **Guides**: Each of the sub-assignments have a corresponding *guide notebook*. Everything needed to complete the assignments is in the notebooks. The guide notebooks are there to help you understand and practice the concepts. Please refer to the table below:

| Assignment | Assignment notebook | Guide notebook | Description |
| --- | --- | --- | --- |
| Part 1 | [assignments/nn.ipynb](assignments/nn.ipynb) | [materials/nns_pytorch.ipynb](materials/nns_pytorch.ipynb) | Artificial Neural Networks |
| Part 2 | [assignments/cnn.ipynb](assignments/cnn.ipynb) | [materials/cnns_pytorch.ipynb](materials/cnns_pytorch.ipynb) | Convolutional Neural Networks |

**Please see due dates and other relevant information in the assignment description on Canvas.**

## Getting started
Please see the relevant sections in the `Development setup guide` document on Canvas for instructions. To iterate, you need to:

1. Fork this repository to your own GitHub account.
2. Clone the forked repository to your local machine.
3. Create a virtual environment and install the required packages.
4. Start working on the assignment.
5. Commit and push your changes to your GitHub repository.
6. Submit a link to your GH assignment repo on Canvas.

## Part 1: Artificial Neural Networks
In this assignment, your task is to construct an MLP architecture for the well-known [MNIST dataset](https://www.kaggle.com/datasets/hojjatk/mnist-dataset).

* Read through the `material/nns_pytorch.ipynb` notebook to understand the basics of PyTorch and how to build a simple neural network.
* Build a n-layer MLP (artificial neural network) in the `assignments/nn.ipynb` notebook

    * Create the architecture (section 4)
    * Set the training parameters (section 5)
    
* See how good a model you can build!

Feel free to play around with the model architecture and see how the training time/performance changes, but to begin, you can try the following:

* Input Layer: Image (784 dimensions) ->  
* Fully connected layer (500 hidden units) -> 
* Nonlinearity (ReLU) ->  
* Fully connected (10 hidden units - digits 0-9) -> 

*Some hints*:
- To get the best performance, you may want to play with the learning rate and the number of training epochs.
- A flattened image of size 28x28 is 784 dimensions. This is the input to the network.

***

## Part 2: Convolutional Neural Networks
In this assignment, your task is to build a CNN architecture for multi-class classification on the famous [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html). 

* Read through the `material/cnns_pytorch.ipynb` notebook to understand the basics of how to build a convolutional neural network.
* Build a n-layer CNN in the `assignments/cnn.ipynb` notebook.

    * Create the architecture (section 4)
    * Set the training parameters (section 5)

* See how good a model you can build!

Feel free to play around with the model architecture - add, layers, adjust layer parameters etc. - and see how the training time/performance changes. Try to get the best performance you can!

You can start with the following:

* 2D Convolutional layer
* Non-linearity (ReLU)
* Max pooling layer
* Flatten the output from the last convolutional layer (this part is already given in the code)
* Fully Connected Layer with 128 hidden units
* Non-linearity (ReLU)
* Fully Connected Layer (output layer for 10 classes)

*Some hints*:
- You need to define the number of filters (also known as channels) in each convolutional layer. Try starting with a small number (e.g., 16 or 32) and increase it in deeper layers.
- The kernel size determines how much of the image each filter sees at a time. Smaller kernels (like 3x3) are commonly used and work well.
- Pick a small number for stride and padding. Padding helps preserve the spatial size of the input, and stride determines how much the kernel moves.
- Pooling layers reduce the spatial dimensions of the feature maps and help reduce computation and overfitting. A common choice is to use 2x2 max pooling with a stride of 2, which halves the spatial dimensions.
<br>
<br>
