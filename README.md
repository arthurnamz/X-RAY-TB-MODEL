# X-RAY-TB-MODEL
Detecting tuberculosis from X-ray scan using pytorch

## Introduction
Dataset is obtained from here which consisted of 2 differnet set of scans, ChinaSet and Montgomery.

ChinaSet consists of 662 scans (including positive and negative cases of TB)
Montogomery consists of 138 scans (including positive and negative cases of TB)
In total there are 800 scans with 394 positive cases and 406 negative cases

I randomly picked 680 scans (85%) for training and 120 scans (15%) for testing.

##Preprocessing of dataset
Each of the scan in training set is randomly rotated, translated, and horizontally flipped to perform the augmentation. No augmentation was performed on testing set. All the scans and their augmented versions for training are present in data/train and test dataset is present in data/test

Preprocessing notebook can be found at src/Xray_DatasetPreprocess.ipynb

Some examples of positive scan and it's augmented version:
