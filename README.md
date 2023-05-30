# Image_colorization

The task is to convert grayscale images to coloured images using OpenCV and CNN.
The dataset consists of 25000 images in the LAB colorspace. The input in the grayscale images and the required output is RGB images which can be obtained from the LAB images. 
Since the dataste is very big, I have implemented the models on a subset of 400 images.
Two approaches have been taken:
1. Initially implemented an autoencoder with convolutional layers on the mean normalized data, got an accuracy of about 51%.
2. Used preprocess_input from ResNet to preprocess the images and then implemented an autoencoder again to these images. Got an accuracy of about 64%.

The dataset can be found on kaggle: https://www.kaggle.com/datasets/shravankumar9892/image-colorization
