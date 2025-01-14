---
tags:
  - oci
Index: "[[4. Deep Learning Foundations]]"
---
# Transcript
In this lesson, we will learn about deep learning. So let's begin. Deep learning is a subset of machine learning that focuses on training artificial neural networks to solve a task at hand, say, for example, image classification. A very important quality of the ANN is that it can process raw data like pixels of an image and extract patterns from it. These patterns are treated as features to predict the outcomes. Let us say we have a set of handwritten images of digits 0 to 9.

As we know, every one writes the digits in a slightly different ways. So how do we train a machine to identify a handwritten digit? For this, we use ANN. ANN accepts image pixels as inputs, extract patterns like edges and curves and so on, and correlates these patterns to predict an outcome, that is, what digit does the image has in this case. In short, given a bunch of pixels, ANN is able to process pixels data, learn an internal representation of the data and predict outcomes.

We need to specify features while we train machine learning algorithm. With deep learning, features are automatically extracted from the data. Internal representation of features and their combinations is built to predict outcomes by deep learning algorithms. This may not be feasible manually. Deep learning algorithms can make use of parallel computations. For this, usually, data is split into small batches and process parallely. So these algorithms can process large amount of data in a short time to learn the features and their combinations.

This leads to scalability and performance. In short, deep learning complements machine learning algorithms for complex data for which features cannot be described easily. Let us quickly look at the history of deep learning. Some of the deep learning concepts like artificial neuron, perceptron and multi-layer perceptron existed as early as 1950s. One of the most important concept of using backpropagation for training and came in 1980s.

In 1990s, convolutional neural network were also introduced for image analysis task. Starting 2000, GPUs were introduced, and 2010 onwards, GPUs became cheaper and widely available. This fueled the widespread adoption of deep learning uses like computer vision, natural language processing, speech recognition, text translation, and so on.

In 2012, major networks like AlexNet and Deep Q-Network were built. 2016 onward, generative use cases of the deep learning also started to come up. Today, we have widely adopted deep learning for a variety of use cases, including large language models and many other types of generative models.

Deep learning algorithms are targeted at a variety of data and applications. For data, we have images, videos, text, and audio. For images, applications can be image classification, object detection and so on. For textual data, applications are to translate the text or detect a sentiment of a text. For audio, the applications can be music generation, speech to text, and so on.

Selecting the right deep learning algorithm based on the data and application is important. For image, task like image classification, object detection, image segmentation, or facial recognition, CNN is a suitable architecture. For text, we have a choice of the latest transformers or LSTM or even RNN. For a generative task like text summarization, question answering, transformers is a good choice. For generating images, text-to-image generation, transformers, GANs, or division models are available choice.

So let us understand what is artificial neural network or ANN. Artificial neural networks are inspired by the human brain. They are made up of interconnected nodes called as neurons. Let us get a simplified understanding of how inputs are processed by a neuron. In ANN, we assign weights to the connection between neurons. Weighted inputs are added up. And if the sum crosses a specified threshold, the neuron is fired, and the outputs of a layer of neuron become an input to an another layer. Let us also understand the building blocks of ANN.

So first building block is layers. We have input layer, output layer, and multiple hidden layers. The input layer and output layer are mandatory. And the hidden layers are optional. The second unit is neurons. Neurons are computational units, which accept an input and produce an output. Weights determine the strength of connection between neurons. So the connection could be between input and a neuron, or it could be between neuron and another neuron.

Activation functions work on the weighted sum of inputs to a neuron and produce an output. Additional input to the neuron that allows a certain degree of flexibility is called as a bias. Now, having understood the components of the ANN, let's also take one small example and see how to train an to recognize handwritten digits from images. For that, we have to collect a large number of digit images, and we need to train ANN using these images.

Now, let us see how do we train ANN using images. So in this case, the images consist of 28 by 28 pixels, which act as a input layer. For the output, we have neurons, 10 neurons, which represent digits 0 to 9, and we have multiple hidden layers. So in this case, we have two hidden layers which are consisting of 16 neurons each. The hidden layers are responsible for capturing the internal representation of the raw image data, and the output layer is responsible for producing the desired outcomes.

So in this case, the desired outcome is the prediction of whether the digit is 0 or 1 or up to digit 9. So how do we train this particular? So the first thing-- we use, the backpropagation algorithm. During training, we show an image to the ANN. Let us say it is an image of digit 2. So we expect output neuron for digit 2 to fire. But in real, let us say output neuron of a digit 6 fired. So what do we do? We know that there is an error.

So to correct an error, we adjust the weights of the connection between neurons based on a calculation, which we call as backpropagation algorithm. By showing thousands of images and adjusting the weights iteratively, ANN is able to predict correct outcome for most of the input images. This process of adjusting weights through backpropagation is called as model training. Thanks for listening.