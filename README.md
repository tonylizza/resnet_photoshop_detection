# Photoshopped Image detection

A pretrained Resnet model using PyTorch that determines whether or not images are photoshopped that has been trained on a dataset from r/ps-battles.

## Data Download

Use the download.sh shell script file and the originals.tsv and photoshops.tsv tab separated files to download original and photoshopped images. Credit goes to user dbisUnibas for the dataset, as well as the implementation of the download.sh script.

## Model

The model uses a pretrained Resnet-50 model and approx 11000 original images and 18000 photoshopped images obtained from the PS-Battles dataset (https://arxiv.org/pdf/1804.04866.pdf) to determine whether or not photos have been retouched. The photos are split 80/20 into training and test sets with 3 epochs, achieving an accuracy of 67.8% on the test set. Future experiments will compare Restnet-50 to other pre-trained models, as well as non-pre-trained models for accuracy and precision.

- Requires NumPY, PIL, and PyTorch
