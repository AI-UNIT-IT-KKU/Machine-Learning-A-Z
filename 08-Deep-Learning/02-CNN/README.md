🐱🐶 CNN for Cat vs Dog Image Classification
📌 Overview

This project uses a Convolutional Neural Network (CNN) to classify images of cats and dogs.
The CNN is trained on labeled images and can predict unseen images with high accuracy.

⚙️ Steps in the Code

Import Libraries → tensorflow (Keras), ImageDataGenerator, numpy.

Data Preprocessing →

Training images: rescale, shear, zoom, horizontal flip (augmentation).

Test images: rescale only.

Resize all images to 64x64 pixels, batch size = 32.

Build CNN → 2 convolutional layers + max pooling, flatten, dense hidden layer (128 units, ReLU), output layer (1 unit, Sigmoid).

Compile CNN → Optimizer: Adam, Loss: Binary Crossentropy, Metric: Accuracy.

Train CNN → 25 epochs with training and validation sets.

Single Image Prediction → Preprocess a single image, predict if it’s a cat or dog.

🎯 Importance

CNNs automatically extract features from images.

Useful for applications like object detection, medical imaging, autonomous vehicles.

Data augmentation improves generalization and reduces overfitting.
