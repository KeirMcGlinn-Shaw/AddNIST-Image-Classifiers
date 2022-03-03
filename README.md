# AddNIST-Image-Classifiers
A collection of three classifiers for classifying images from the AddNIST dataset  

Data
The dataset is the AddNIST1 dataset from https://github.com/RobGeada/cvpr-nas-datasets.
Each image is a composition of three MNIST digits one in each of the three colour channels.
Some examples are given in Figure 1.

![Example image](assets/AddNIST-Example-Data-Image.png)
Figure 1: Examples of the AddNIST dataset. Each image (the large image) is made up of
three MNIST images â€“ one in each of the three colour channels. The label for the image is
the sum of the three numbers and then subtract 1. So, for example the top left image is r=3,
g=2, b=4 and the label is r+g+b-1 = 8.
There are six datafiles: All available on Canvas
Filename A numpy dataframe containing:
train_x.npy 45,000 training example images
train_y.npy 45,000 labels for the data in train_x.npy
valid_x.npy 15,000 more images for validation
valid_y.npy 15,000 more labels matching valid_x.npy
test_x.npy 10,000 more images for testing
test_y.npy 10,000 more labels matching test_x.npy
