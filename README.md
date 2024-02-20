# Introduction
The task intended to be solved is image classification and the provided solution consists of the fine-tuning of ResNet50, a popular convolutional neural network pre-trained on ImageNet.<br>
Four files are provided:
- Training.ipynb;
- Test_Inference.ipynb;
- weights_30.pth;
- test_set_predictions.csv.

The files must be placed on a folder containing TRAINING.zip and TEST.zip.
Please notice that the two Jupyter Notebooks contain instructions for mounting and entering my personal Google Drive folder with the files necessary for running the notebooks themselves. Therefore, if one wants to run them, those lines must be changed. Moreover, there are also the instructions to unzip the TRAINING.zip and TEST.zip folders, if not already done.

# Training.ipynb
This notebook basically contains:
- the implementation of the class to load training images both in a training set and in a validation set;
- the creation of a training set and a validation set with images in the TRAINING folder with respective dataloaders;
- the loading of ResNet50 pre-trained model on ImageNet-1K and its slight modification to make it suitable for our task;
- the fine-tuning of the model on the loaded training set.

# Test_Inference.ipynb
This notebook includes:
- the creation of the file test_set_predictions.csv with names and inferred labels for images in the TEST folder;
- a function that allows the user to plot each image in the TEST folder with its predicted label.

# weights_30.pth
The file containing trained weights of the model, to be used for inference.

# test_set_predictions.csv
This is the required file after model inference on the images in TEST. Basically, each line consists of two values: the name of an image and the label the model assigned to it.