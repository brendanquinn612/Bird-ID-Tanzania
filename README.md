# Bird-ID-Tanzania

A convolutional neural network that can label pictures of the birds of Tanzania.

![Birds](https://i.ibb.co/W3P7mvm/intro.png)

## The Problem

Tanzania is home to 1116 species of birds. Quickly identifying them can be challenging for experts, let alone novices in the field. Great strides have been made to try and identify wildlife with neural networks, but none have focused on Tanzania. This project tackles both issues.

![NN Layer Types](https://i.ibb.co/1TW49vh/vgg-overview.png)

## Data & Model

This project used over 57,000 pictures of bird acquired via the Flickr API. They were stored on an AWS S3 bucket and processed using TensforFlow on Google Colab. The final model was a VGG-19 pre-trained on ImageNet.

![VGG diagram](https://i.ibb.co/qFNFRv9/vgglayers.png)

## Results

The model currently has an accuracy of 20%. That does not sound great at first glance, but if the model guessed randomly it would only have an accuracy of 0.089%. The performance of the model could have been improved if I used a more powerful model such as Xception, or had more cloud resources to train the model with.

Another issue is that many birds look quite similar. The model identified each pair below as being of the same species, but each of the 8 pictures is of a unique species. 

![Bird Pairs](https://i.ibb.co/f1Znr9Q/pairs.png)

## Next Steps

A more robust model with much more training time would greatly boost accuracy. The pairing problem could be solved by supplementing the neural network with basic questionaires asking questions like the approximate size or habitat the bird was in. 

![More Birds](https://i.ibb.co/T006k7w/outro.png)
