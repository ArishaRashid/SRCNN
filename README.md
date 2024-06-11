In this project we implement single image super resolution using CNN, by reproducing a research paper Learning a Deep Convolutional Network for Image Super-Resolution by Dong et al. (2014)

Single image super-resolution (SR) is a classical computer vision problem that aims at recovering a high-resolution image from a lower resolution image. There are example based methods to solve it, such as mapping or using internal similarities but we looked into a method proposed by Dong et. al

In this project, we use a technique called Super Resolution Convolutional Neural Network. This technique work end to end by extacting patches from the low resolution image and passing them throw convolutional layers to final map them to higher resolution output pixels, as shown in the diagram below.

We implemented the SRCNN model in TensorFlow, trained it and then tested it on a low resolution image.

Given a low-resolution image Y, the first convolutional layer of the SRCNN extracts a set of feature maps. The second layer maps these feature maps nonlinearly to high-resolution patch representations. The last layer combines the predictions within a spatial neighbourhood to produce the final high-resolution image F(Y). (Dong et al.,2014)

As an image dataset for training the model, we will be using a Kaggle hosted dataset called Dog and Cat Detection.
