# Bird-ID-Tanzania

A convolutional neural network that can label pictures of the birds of Tanzania.

Tanzania is home to 1116 species of birds. That can make for difficult identifications in the field. Machine learning can be used to recognize birds through photography. 

This project used over 57,000 pictures of bird acquired via the Flickr API. They were stored on an AWS S3 bucket and processes using TensforFlow on Google Colab. Due to time constraints, I used a VGG-19 model that was pretrained on ImageNet. The final model had about 205 accuracy. The baseline for all species was less than a tenth of a percent, so that represents a substantial move in the right connection.
