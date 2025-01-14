---
Index: "[[2. AI Foundations]]"
tags:
  - "#oci"
---
# Transcript 

Let's focus on AI tasks and data pertaining to these three AI domains. We have language, audio and speech, and vision. Let's begin with language tasks. Language-related AI tasks can be text-related or generative AI. Text-related tasks, use text as input, and the output can vary depending on the task. Some examples include detecting language, extracting entities in a text, or extracting key phrases and so on.

Consider the example of translating text. There's many text translation tools where you simply type or paste your text into a given text box. Choose your source and target language, and then click translate. Now let's look at the generative AI tasks.

They are generative, which means the output text is generated by a model. Some examples are creating text like stories or poems, summarizing a text, answering questions, and so on. Let's take the example of ChatGPT, the most well-known generative chat bot. These bots can create responses from their training on large language models, and they continuously grow through machine learning. Let's look at how text as data works.

Text is inherently sequential, and text consists of sentences. Sentences can have multiple words, and those words need to be converted to numbers for it to be used to train language models. This is called tokenization. Now the length of sentences can vary. And all the sentences lengths need to be made equal. This is done through padding.

Words can have similarities with other words, and sentences can also be similar to other sentences. The similarity can be measured through dot similarity or cosine similarity. We need a way to indicate that similar words or sentences may be close by. This is done through representation called embedding. Now let's take a look at various language AI models.

Language AI models refer to artificial intelligence models that are specifically designed to understand, process, and generate natural language. These models have been trained on vast amounts of textual data that can perform various Natural Language Processing, or NLP tasks. The task that needs to be performed, the size, the type of input and output.

The deep learning model architectures that are typically used to train models that perform language tasks are recurrent neural networks, which processes data sequentially and stores hidden states, long short-term memory, which processes data sequentially that can retain the context better through the use of gates, and transformers, which processes data in parallel. It uses the concept of self-attention to better understand the context.

Speech-related AI tasks can be either audio-related or generative AI. Speech related AI tasks use audio or speech as input, and the output can vary depending on the task. For example, speech-to-text conversion, or speaker recognition, voice conversion, and so on. Generative AI tasks are generative in nature, so the output audio is generated by a model. For example, you have music composition and speech synthesis.

Audio or speech is digitized as snapshots taken in time. The sample rate is the number of times in a second an audio sample is taken. Most digital audio have a sampling rate of 44.1 kilohertz, which is also the sampling rate for audio CDs. This means that the audio is sampled 44,100 times per second during recording. And when the audio is played, the hardware then reconstructs the sound 44,000 times per second.

The bit depth is the number of bits in each sample or how information rich of each of those 44,000 pieces of audio is. However, nothing much can be inferred by looking at just one audio sample. Multiple samples need to be correlated to make sense of the data. For example, listening to for a fraction of a second, you won't be able to infer much about the song, and you'll probably need to listen to it a little bit longer.

Audio and speech AI models are designed to process and understand audio data, including spoken language. These deep learning model architectures are used to train models that perform language tasks-- recurrent neural networks, long short-term memory, transformers, variational autoencoders, waveform models, and Siamese networks. All of the above models take into consideration the sequential nature of audio.

Vision-related AI tasks could be image-related or generative AI. Image-related tasks will use an image as an input, and the output depends on the task. Some examples are classifying images, identifying objects in an image, and so on. Facial recognition is one of the most popular image-related tasks that is often used for surveillance and tracking of people in real time. And it's used in a lot of different fields, including security, biometrics, law enforcement, and social media.

For generative AI tasks, the output image is generated by a model. For example, creating an image from a contextual description, generating images of a specific style or a high resolution, and so on. It can create extremely realistic new images and videos by generating original 3D models of an object, machine components, buildings, medication, people and even more.

Images as data. Images consist of pixels and pixels can be either grayscale or color, and we can't really make out what an image is just by looking at one pixel. The task that needs to be performed, decides the type of input needed and the output produced. Various architectures have evolved to handle this wide variety of tasks and data. These deep learning model architectures are typically used to train models that perform vision tasks.

Convolutional neural networks, which detects patterns in images, learning hierarchical representations of visual features. YOLO, which is You Only Look Once, processes the image and detects objects within the image. And then you have generative adversarial networks, which generates real-looking images.

Some other AI tasks. Anomaly detection. This is time series data, which is required for anomaly detection, and it can be a single or multivariate for fraud detection, machine failure, et cetera. Recommendations. You can recommend products using data of similar products or users. For recommendations, data of similar products or similar users is required. Forecasting. Time series data is required for forecasting and can be used for things like weather forecasting and predicting the stock price. Thank you.