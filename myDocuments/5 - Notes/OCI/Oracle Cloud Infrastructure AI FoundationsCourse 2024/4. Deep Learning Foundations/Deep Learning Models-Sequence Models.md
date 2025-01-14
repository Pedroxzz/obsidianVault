---
tags:
  - oci
Index: "[[4. Deep Learning Foundations]]"
---
# Transcript
In this lesson, we will learn about deep learning models that are suitable for processing sequential data, for example, a paragraph of a text. Sequence models are used to solve problems where the input data is in the form of sequences. The sequences are ordered lists of data points or events. The goal in sequence models is to find patterns and dependencies within the data and make predictions, classifications, or even generate new sequences.

Some common examples of the sequence models are, in natural language processing, deep learning models are used for tasks such as machine translation, sentiment analysis, or text generation. In speech recognition, deep learning models are used to convert recorded audio in a text.

And deep learning models can generate new music or create original compositions. Even sequences of hand gestures are interpreted by deep learning models for applications like sign language recognition. In fields like finance or weather prediction, time series data is used to predict future values. Let us see some of the deep learning models which can be used to work with sequence data.

Recurrent Neural Networks, abbreviated as RNNs, are a class of neural network architectures specifically designed to handle sequential data. Unlike traditional feedforward neural network, RNNs have a feedback loop that allows information to persist across different timesteps. The key features of RNN is their ability to maintain an internal state, often referred to as a hidden state or memory, which is updated as the network processes each element in the input sequence. The hidden state is then used as input to the network for the next time step, allowing the model to capture dependencies and patterns in the data that are spread across time.

There are different types of RNN architecture based on application. One of them is one-to-one. This is like feedforward neural network and is not suited for sequential data. A one-to-many model produces multiple output values for one input value. Music generation or sequence generation are some applications using this architecture.

A many-to-one model produces one output value after receiving multiple input values. Example is sentiment analysis based on the review. Many-to-many model produces multiple output values for multiple input values. Examples are machine translation and named entity recognition. RNN does not perform that well when it comes to capturing long-term dependencies. This is due to the vanishing gradients problem, which is overcome by using LSTM model.

Long Short-Term Memory, abbreviated as LSTM, works by using a specialized memory cell and a gating mechanisms to capture long-term dependencies in the sequential data. The key idea behind LSTM is to selectively remember or forget information over time, enabling the model to maintain relevant information over long sequences which helps overcome the vanishing gradients problem. Let us see how LSTM works.

Let us see the step-by-step working of LSTM. At each timestep, the LSTM takes an input vector representing the current data point in the sequence. The LSTM also receives the previous hidden state and cell state. These represent what the LSTM has remembered and forgotten up to the current point in the sequence. The core of the LSTM lies in its gating mechanisms, which include three gates, the input gate, the forget gate, and the output gate. These gates are like the filters that control the flow of information within the LSTM cell.

The input gate decides what new information from the current input should be added to the memory cell. The forget gate determines what information in the current memory cell should be discarded or forgotten. The output gate regulates how much of the current memory cell should be exposed as the output of the current time step.

Using the information from the input gate and forget gate, the LSTM updates its cell state. The LSTM then uses the output to produce the current hidden state, which becomes the output of the LSTM for the next time step. Thanks for watching.