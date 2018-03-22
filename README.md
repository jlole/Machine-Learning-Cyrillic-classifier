# Cyrillic Alphabet Classifier

## Machine Setup
1. Install Python 3
1. Use pip to install the following:
   * Pillow
   * Keras
   * Tensorflow
   * Jupyter (reinstalling might fix some issues)
   * h5py

## Convert files
Since the images in the dataset we use are incompatible with keras, we have to convert them. This script converts the 278x278 rbga? png files into 56x56 rbg images.

This makes the images compatible with keras __and__ smaller to save time.

The reason for the folder names (aa, ab, ..., bg) is that on windows the cyrillic characters do not work correctly and numerical names doesn't stay in the same order in keras.

* from data/training -> data_converted/training
* from data/testing -> data_converted/testing

*Make sure the folders for converted exits, best to make a copy of data and rename it to data_converted to be overwritten*

## Cyrillic Classifier
train network and save to models/<filename>.h5

## Cyrillic Check
open image and insert into model to predict what it is

## Test Instructions
1. Use [this](https://pixlr.com/editor/) or MS paint to create a 56x56 **jpg** with a Cyrillic letter and a white background
1. Save the image (eg: in data_converted/)
1. Open Cyrillic check notebook
1. Run the cell to create the models
1. Run the cell to load the weights into the model
1. Edit the filename of the file to test if needed
1. Run the cell to get the prediction
