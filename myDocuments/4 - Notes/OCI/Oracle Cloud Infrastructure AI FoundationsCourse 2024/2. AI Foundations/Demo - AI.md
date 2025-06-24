---
Index: "[[2. AI Foundations]]"
tags:
  - "#oci"
---
# Transcript 
In this lesson, I'll walk you through a couple of OCI AI services. The first one, Vision AI service. Vision AI service allows us to carry out a few tasks-- image classification, object detection, text detection, and Document AI. Let us explore each one of these.

So let me pick up one local file for the image analysis over here. So, as you can see, the image has been analyzed, and we have got multiple labels here. And this is the confidence score of those labels. So what it means is, for the vegetation, the AI services 99.23% sure that there is a vegetation in this image.

Let's try another image. This time, let's pick up an image of a zebra. So, once again, you can see here that the Zebra has been detected, vegetation, grassland, plant, animal-- all these labels have been assigned with the confidence scores over here.

Let's pick up another image as well. Let's pick up two zebras this time and see what happens. So it recognizes zebra. It also assigned a label of an animal, vegetation, sky, and a mammal. Let's try object detection. Let's pick up one image of a traffic over here.

So in the object detection, we essentially get all these kind of bounding boxes around the objects. And, as you can see here, we have got the labels also and their confidence scores. And as you can see, multiple cars have been detected. Taxi has been detected. Multiple people have been detected into this image. Let's try another one.

So it's a basket of fruit, and you can see here that multiple fruits, including orange, banana, apple have been detected. Even a bowl has been detected over here.

Let's try our text detection. So let's pick up an image of a bus over here. So, as you can see, this bus has a lot of text written on it. So these are all the text that has been written and extracted by the service over here.

It has even detected this number plate M32HOD. It has also detect this number 45 over here, all this text here, text here, and even the text here, and smaller text blocks over here also. Even this has been detected over here.

Let's take another image for our text detection. So I just picked up image of different kind of fonts and I was just curious to see if it is able to extract the text, which is written into different fonts.

So this is how it goes. It basically goes line by line. So Ariel, and the next word you will see is this. Then you will see Ariel Black and the words over here. So like that, it will keep on scanning the whole-- whole image over here.

Now let's try the Document AI also. So one thing about Document AI is Document AI essentially has been moved to a separate service, which is called as document understanding. But from the feature perspective, the features of the Document AI envision and the document understanding service are the same. So let's try one image over here. So I'll upload one receipt over here, and let's see how does it analyze that receipt.

So, as you can see here, this is all the raw text. First, we are able to see there's a lot more to it. So it is essentially from here like starting from receipt to thank you. It has scanned all the words over here. Now, what it has done for the key value-- so what it has done is actually it has picked up the transaction date somewhere over here.

And transaction time also it has picked up. It has picked up the subtotal. It has picked up the tags and the total. These are the standard items. So it has extracted them as a key value pairs also. And then further also line by line, you can see the key value pairs have been extracted over here.

Let's see what kind of tables it has extracted. So if I just click on this drop down, the three tables have been extracted over here. So the first table, as you can see or see over here. Second table is this particular table-- the total. And the third table is the bottom one here-- card, auth code, and other details were like terminal ID and the amount.

So I hope you find this interesting. We will explore OCI AI Language service. As you can see here, we can do two things here. One is the text analysis, and second is text translation. So, in the text analysis, all these pre-trained models, including language detection, text classification, sentiment analysis, and a few others. They are applied to a block of text that we give.

So let's give some text here. Let's say we'll paste some text here, and we'll analyze this text here. And we can see that the first thing it has done is it has detected the language as English. It has classified the paragraph as a science and technology or a computer-related paragraph.

And it has extracted multiple entities. So entities like food and computers and manual instruments, and so on. And they have been tagged as like, say, a product or an event and many other categories. And these are the confidence scores for those entities. And the key phrases for the text also have been extracted over here, say, something like the early computers or simple manual instruments, and so on.

The sentiments also have been detected-- so aspect-based sentiment. So aspect is like one subject in the paragraphs, so something like food or a service and early computers. All the sentiments have been detected, their score, and whether they are negative or positive-- that has been indicated.

And we also have the sentence level sentiments also, which are marked as either negative or neutral in this particular case. And the personal identifiable information has also been identified. So some of the sensitive data like World War II or dates around it, and they have been indicated as potentially could be being sensitive. So that is an indication that the service has given us. That's the-- that is about the text analysis.

Moving on to the text translation. We have a block of text here, and the source language is English here but we can change it to anything depending on the text that we provide. For now, let's keep it as English. And then for the target also, we have a choice of multiple languages here. Let's try the French first.

So if we click translate just in a couple of seconds, the text has been translated and then we can try some other language like Japanese also over here. So the text has been translated into Japanese language also.

And then, if we go to the Overview once again, we also have the capability of training the custom models also over here. If we provide the custom data, we can train our custom models also. Thanks for watching.