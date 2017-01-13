---
layout: post
title: Deep Learning Vocabulary
---

I have built various software applications professionally for many years. I saw an amazing potential in the way lot of problems can be solved using Deep Learning and thought of learning it. Initially, it was an uphill task for me and it took lot of time to build the vocabulary to understand research papers and talk to scientists. Some other engineers I know share the same experience.

### Understanding the vocabulary

I had to learn these definitions from different places, most of my time was spend finding some blog/article which explains it in easy words without lot of long formulas. I prepared the following list as my reference and thought of sharing it so it can be a quick refresher/starting place for engineers learning deep learning.

Of course, this is oversimplified list (in fact, that's the goal of this post) and readers should explore these topics in details as they ramp up.

One Hot encoding
: Representing something with 0s and 1s such that we have 1 only at the place where the category is matching and every other place is 0.

Fine-tuning
: The model learns parameters based on the set of data provided. An existing model is "fine-tuned" to learn new categories. For eg. A model which can identify dog breed can be fine-tuned to identify dogs.

Convolution layers
: Used for finding patterns in images. Each Layer can use previous layers output and can find increasingly more complex patterns.

Dense (fully connected) layers
: Used for combining patterns across an image. Most times Dense Layers are used after Convolution layers.

Relu (Rectified Linear Unit)
: A function while = max (0,1)

Loss Function, Objective function or Cost function
: corresponds to what we care about for optimization.

SGD
: A set of initial points are chosen (lot of ways of choosing them) and a gradient is calculated to reach the minima based on loss function.

Perceptron
: Takes Multiple binary inputs and returns a **single** binary output. It multiplies each binary input with a real weight (w1,w2..etc) and does an aggregated sum.
If the sum is less than a predefined threshold it outputs 0 otherwise 1.

Sigmoid neuron
: Takes multiple inputs between 0 and 1 and returns an output **between** 0 and 1. A small change in inputs and weights results in only small change in output. Also called log function since the formula is 1/1+e^-z ( where z =  Sum(inputs.weights + bias)

Hidden Layer
: A layer which is not input or output.

Feedforward neural networks
: Neural nets where the output from previous layer is fed as input into the next layer. Its only uni-directional.

Recurrent Neural Network
: Unlike Feedforward Networks, some of the Neurons can be fired multiple times in a loop and use information from previous firing.

Imperative programs
: Easy to understand, not flexible for optimization. Executes step by step and all the intermediate variables hold the data.

Declarative programs
: Good optimizations since the data is fed/injected after the calculation is defined. Generally an opration is defined generically and then a compile operation is done. Data is fed into the compiled function and it returns output optimizing all intermediate steps. Not very flexible, If a change is made it needs recompilation.

Activation function
: it defines the output of a neuron for a given set of inputs.

Max Pooling
: Takes each block of area and finds brightest pixel in each block. It allows downsampling of the original data and avoid overfitting. Similarly we call it Average pooling if the downsampling is done using the average of the block.

Support Vector Machine
:

Regularization
: Techniques to prevent the network from Overfitting (where the model works extrememly well for test data since it has learnt the data and has not generalized)

Dropout
: A type of regularization where some of the neurons and their connections are removed randomly. This helps avoid overfitting since each network is different.

L1 regularization
:

L2 regularization
:

Ensemble Learning
: A collection of models are used together to predict outcome.

auto differentiation, or backpropagation
:

operation folding
:

Factorization Machines
:

K Means
:

matrix Factorization
:

Matrix decomposition
:

Hyper Parameter Tuning
:

Beam search
: Optimized Breadth first search where only a subset of choices are kept/traversed depending on the cost function and it provides a heuristics based answer.

Shilling attack
: Also called Profile injection attack, Someone/Competitors may inject fake user profiles to confuse Collaborative filtering systems.
