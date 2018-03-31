# Cyrillic Alphabet Classifier

## Machine Setup
1. Install Python
1. Use pip to install the following:
   * Pillow
   * Keras
   * Tensorflow
   * Jupyter (reinstalling might fix some issues)
   * h5py

## Convert files
Since the images in the dataset we use are incompatible with keras, we have to convert them. This script converts the 278x278 rbga? png files into 28x28 rbg images.

This makes the images compatible with keras __and__ smaller to save time while training the network.

This notebook takes images from data/combined and splits it up into data/testing and data/training

data/testing will contain 100 images per character and data/training will contain variable amounts depending on the ratio.

## Cyrillic Classifier
train network and save weights to models/Model<number>.h5

## Cyrillic Check
open image and insert into model to predict what it is
there are images in data/predict to test