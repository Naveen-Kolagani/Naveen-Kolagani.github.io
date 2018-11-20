# Naveen-Kolagani.github.io

## Devanagari-Handwritten-Character-Recognition
### This repo explains the recognition of Devanagari handwritten characters
#### INCEPTION V3 PRE-TRAINED Model is used for training the classifier
[Link](https://archive.ics.uci.edu/ml/datasets/Devanagari+Handwritten+Character+Dataset#) to the dataset
#### The images are of 32x32 size
##### The whole is dataset is divided into 60, 20, 20 percentages for training, testing and validation.
#### For reducing computational complexity and time complexity trasnsfer learning is used by making use of a pre-trained [INCEPTION V3 Model](http://download.tensorflow.org/models/image/imagenet/inception-2015-12-05.tgz)

## Requirements
- GPU (For faster computation) or
- [Google Colaboratory](https://colab.research.google.com/drive/1yG2Zk66IdIoknFmsmsaENKCSfuhHxO-a)
- Tensorflow
- NumPy

## Process of Training

- Bottlenecks files are created for each image and these values are used for training purpose
- During the training these bottleneck values are taken at random from training set and fed to the pre-trained model in batches of size 100
- The bottleneck files are covoluted with the weights in the last layer of pre-trained model and weights are updated
- The weights are updated in the backpropagation step

#### The model gives an test accuracy of 84% and a training accuracy of 87%
![Training Accuracy Image](https://github.com/Naveen-Kolagani/Devanagari-Handwritten-Character-Recognition/blob/master/Accuracy.png)
![Predictions from the above model](https://github.com/Naveen-Kolagani/Devanagari-Handwritten-Character-Recognition/blob/master/Predictions.png)
#### This model lets you add distortions to the images for better training.
#### For better visualization the jupyter notebook summarizes the logs and they can be visualized with Tensorboard

![Network Model](https://github.com/Naveen-Kolagani/Naveen-Kolagani.github.io/blob/master/Network%20Model.png)
![Cross-Entropy](https://github.com/Naveen-Kolagani/Naveen-Kolagani.github.io/blob/master/cross-entropy.png)
![Summary 1](https://github.com/Naveen-Kolagani/Naveen-Kolagani.github.io/blob/master/summary-1.png)
![Summary 2](https://github.com/Naveen-Kolagani/Naveen-Kolagani.github.io/blob/master/summary-2.png)
