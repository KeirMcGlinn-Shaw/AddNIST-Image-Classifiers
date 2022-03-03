# AddNIST-Image-Classifiers
A collection of three classifiers for classifying images from the AddNIST dataset  

## Data
The dataset used in this prokect is the AddNIST1 dataset which can be found in this repository https://github.com/RobGeada/cvpr-nas-datasets.
Each image is a composition of three MNIST digits one in each of the three colour channels, and the labels for the images are the sum of the three digits contained within the image minus 1. Some examples are given in Figure 1.

![Example image](assets/AddNIST-Data-Image.png)
### Figure 1: Examples of the AddNIST dataset.

Each image (the large image) is made up of three MNIST images one in each of the three colour channels. The label for the image is the sum of the three numbers and then subtract 1. So, for example the top left image is r=3, g=2, b=4 and the label is r+g+b-1 = 8. There are six datafiles: All can be generated from the [cvpr-nas-datasets repository](https://github.com/RobGeada/cvpr-nas-datasets).

| Filename      | A numpy dataframe containing              |
| ------------- | ----------------------------------------- |
| train_x.npy   | 45,000 training example images            |
| train_y.npy   | 45,000 labels for the data in train_x.npy |
| valid_x.npy   | 15,000 more images for validation         |
| valid_y.npy   | 15,000 more labels matching valid_x.npy   |
| test_x.npy    | 10,000 more images for testing            |
| test_y.npy    |  10,000 more labels matching test_x.npy   |

The dataset is constructed in such a way that there are only 20 possible ‘classes’ for the prediction – the numbers 0 through 19. In no scenario should the answers add up to less than zero or more than 19.
