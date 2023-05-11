# vgg16, ResNet50 classifier with grad-cam

## Description
Using vgg16 and ResNet50 to classify images and generate a heat map using grad cam.

## Training
- For ResNet50, we are using the pre-trained model available in tensorflow.keras
- For VGG16, we manually train the model using the ImageNet dataset.

### GradCam
We use the last convolutional layer('conv5_block3_out') to generate a heat-map

### Examples
![ResNet50 example](https://github.com/AmiraliEsi83/ImageNet-data-base/blob/main/Examples/ResNet50-Car-Heat-Map.png?raw=true)
![ResNet50 example](https://github.com/AmiraliEsi83/ImageNet-data-base/blob/main/Examples/ResNet50-Burger-Heat-Map.png?raw=true)

### Files
Notebook Files:

- Final_ResNet50_GradCam.ipynb
    - Loads ResNet50 model trained on ImageNet
    - Loads an image from the drive
    - prints the top 5 predictions
    - Generates a heat map based on the top prediction

- vgg16onIMAGENET.ipynb
    - Loads the ImageNet dataset
    - Adds the layers to the model
    - Trains the model
    - Generates heat map based on the top prediction