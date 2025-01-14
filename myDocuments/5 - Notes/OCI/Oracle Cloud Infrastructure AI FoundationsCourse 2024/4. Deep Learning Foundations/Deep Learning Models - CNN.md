---
tags:
  - oci
Index: "[[4. Deep Learning Foundations]]"
---
# Transcript
Welcome to a new lesson. In this lesson, we will learn about Convolutional Neural Networks, abbreviated as CNN. Let us get an overview of deep learning model architectures. The first one is Feedforward Neural Networks, abbreviated as FNN. This is also called as Multilayer Perceptron as MLP and is the simplest form of neural networks.

Second is CNN, which is Convolutional Neural Network. This can automatically detect and learn local patterns and features in images and videos. The third one is RNN, which is a recurrent neural network. RNNs are designed to handle sequential data, such as time series data or natural language. They have a feedback loop that allows them to maintain hidden states and capture temporal dependencies.

The fourth one is autoencoders. Autoencoders are unsupervised learning models used for feature extraction and dimensionality reduction and is commonly employed in data compression and anomaly detection. The fifth one is LSTM. That is long short-term memory. LSTM is a specialized RNN variant designed to handle long-term dependencies in sequential data.

The sixth one is GAN, which is Generative Adversarial Network. This is a powerful, deep learning model, which is used for generating realistic synthetic data such as images, audio, and text. And the last one is transformers. Transformers are widely used in natural language processing and have become state-of-the-art models for tasks like machine translation, text generation, and language understanding. In this lesson, we will go deeper into the understanding of CNN.

So what is a convolutional neural network? CNN is a type of deep learning model specifically designed for processing and analyzing grid-like data such as images and videos. In the ANN, which was seen in the previous lesson, the input image is converted to a single dimensional array and given as an input to the network. But that does not work well with the image data because image data is inherently two-dimensional.

CNN works better with two-dimensional data. The role of the CNN is to reduce the image into a form, which is easier to process and without losing features, which are critical for getting a good prediction. Let us see how this happens using a CNN architecture.

Let us get an overview of the CNN layers. The first one is input layer. Input layer is followed by feature extraction layers, which is a combination and repetition of multiple feature extraction layers, including convolutional layer with ReLU activation and a pooling layer. And this is followed by a classification layer. These are the fully connected output layers where the classification occurs as a output classes. The feature extraction layers play a vital role in image classification. Let us see what happens in that layer with an example.

In order to understand feature extraction layers better, let us take an analogy. Let us say we have a robot to inspect a house and tell us what type of a house it is. It uses many tools for this purpose. The first tool is a blueprint detector. It scans different parts of the house like walls, floors, or windows and looks for specific patterns or features. The second tool is a pattern highlighter. This tool marks areas detected by the blueprint detector. The next tool is a summariser. It tries to capture the most significant features of every room.

The next tool is house expert, which looks at all the highlighted patterns and features and tries to understand the kind of the house. The next tool is a guess maker. It assigns probabilities to the different possible house types. And finally, the quality checker randomly checks different parts of the analysis to make sure that the robot doesn't rely too much on any single piece of information. Let us see how this is mapped to the feature extraction layers.

Let us check the analogy between a robot, house inspector, and different layers of the feature extraction. Similar to blueprint detector, we have a convolutional layer. This layer applies convolutional operations to the input image using small filters known as kernels. Each filter slides across the input image to detect specific features, such as edges, corners, or textures.

Similar to pattern highlighter, we have an activation function. The activation function allows the network to learn more complex and non-linear relationships in the data. Pooling layer is similar to room summarizer. Pooling helps reduce the spatial dimensions of the feature maps generated by the convolutional layers. Similar to a house expert, we have a fully connected layer, which is responsible for making final predictions or classifications based on the learned features.

Softmax layer converts the output of the last fully connected layers into probability scores. The class with the highest probability is the predicted class. This is similar to the guessmaker. And finally, we have the dropout layer. This layer is a regularization technique used to prevent overfitting in the network. This has the same role as that of a quality checker.

To summarize, the purpose of feature extraction layers is to automatically learn and extract relevant patterns and features from the input images. Convolutional layer applies convolutional operations to the input image using small filters known as kernels. Each filter slides across the input image to detect specific features, such as edges, corners, or textures.

The second one is the activation function, which is applied after each convolutional operation. The activation function allows the network to learn more complex and non-linear relationships in the data. And the third one is pooling. It helps reduce computational complexity and also reduces the spatial dimensions of the feature maps generated by the convolutional layers.

CNNs do have some limitations that are important to be aware of. Training CNNs on large data sets can be computationally expensive and time-consuming. CNNs are susceptible to overfitting, especially when the training data is limited or imbalanced. CNNs are considered blackbox models, making it difficult to interpret. And CNNs can be sensitive to small changes in the input leading to unstable predictions.

One of the most widely used applications of CNNs is image classification, for example, classifying whether an image contains a specific object, say, cat or a dog. CNNs are used for object detection tasks. The goal here is to draw bounding boxes around objects in an image.

CNNs can perform pixel level segmentation, where each pixel in the image is labeled to represent different objects or regions. CNNs are employed for face recognition tasks as well, identifying and verifying individuals based on facial features. CNNs are widely used in medical image analysis, helping with tasks like tumor detection, diagnosis, and classification of various medical conditions.

CNN's play an important role in the development of self-driving cars, helping them to recognize and understand the road traffic signs, pedestrians, and other vehicles. And CNN are applied in analyzing satellite images and remote sensing data for tasks such as land cover classification and environmental monitoring. Thanks for watching.