# Mating Detector

A Object-Detection program based on the Faster R-CNN architecture to detect mating-events from mitochondria of yeast cells in microscopic pictures

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

 * Python 3.3+
 * Tensorflow >= 1.6
 * OpenCV
 * pycocotools
 * Cell Data: download here:


### Initialition

Change the Config-File:

When training on the yeast cell data:

 * Change the data path

When training on own data:

 * Change the data path
 * Change categories number and names
 * Adjust Anchor sizes (and so on)


## Running the training

Run the script from the command line by:

```
./train.py [--config \
    MODE_MASK=True MODE_FPN=True \
    DATA.BASEDIR=/path/to/COCO/DIR \
    BACKBONE.WEIGHTS=/path/to/ImageNet-R50-AlignPadding.npz]
```

### Predict an image

Open the Jupyter Notebook: 

```
'predict_and_visualize.ipynb'
```

and follow the instructions:

First change the directory, where to find the image for prediction and  where to save the predicted image.

Run the Notebook from the beginning.


## Authors

* **Leonie Ganswindt** 


## Acknowledgments

* Used code: https://github.com/tensorpack/tensorpack/tree/master/examples/FasterRCNN

