# Facial Expression Detection
This article will demostrate how to create a simple facial expression detection using transfer learning.
In this we will use VGG16 as a pretrained model, on the top of this model we will Create our Facial expression detector.

And also we will use google colab for training the model.
## Requirments

 1. tensorflow 2.x
 2. Keras
 3. Pillow
## Google Colab setup
- 1- First upload the dataset on your google drive, Create a new colab file and mount your google drive to your google colab workspace.
![mount](https://github.com/narayanhari/FacialExpressionDetector/blob/master/mount.PNG)

- Now copy the dataset to your workspace
> !cp -r "/content/drive/My Drive/facial Recoge Dataset" .

Now setup is complete
## Now Code for Model Traning
Import all the libraries first and download vgg16 model
![import](https://github.com/narayanhari/FacialExpressionDetector/blob/master/1.PNG)

setup enviormental variable and change model output layer and create a new model
![model](https://github.com/narayanhari/FacialExpressionDetector/blob/master/2.PNG)

Freeze all the layer except the last output layer
![freeze](https://github.com/narayanhari/FacialExpressionDetector/blob/master/3.PNG)

Import all the the dataset from directory and use augmatation on the images
![dataset](https://github.com/narayanhari/FacialExpressionDetector/blob/master/4.PNG)

Compile the model and train it
![train](https://github.com/narayanhari/FacialExpressionDetector/blob/master/5.PNG)

Save the model and import testing image
![save model](https://github.com/narayanhari/FacialExpressionDetector/blob/master/6.PNG)

Predict the output
![predict](https://github.com/narayanhari/FacialExpressionDetector/blob/master/7.PNG)
