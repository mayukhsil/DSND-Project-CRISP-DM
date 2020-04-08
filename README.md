# DSND-Project-CRISP-DM
### Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing)

# Installation <a name="installation"></a>
#### The packages included in the Annaconda distribution, along with the below libraries must be installed before running.
 Tensorflow
 Sklearn
 Opencv
 Pandas
 Numpy
 Seaborn

# Project Motivation<a name="motivation"></a>

For this project, I was interestested in using COVID-19 data from Kaggle to better understand:

1. What Are The Top 10 Countries In Terms Of Confirmed Cases And Fatalities?
2. What Are The Top States In Terms Of Confirmed Cases In China And US ?
3. Which Country Is Able To Control The Spread Of COVID-19 ?

# File Descriptions<a name="files"></a>

## Dataset
The dataset was collected from many sources. Currently this git repo is maintaining the COVID-19 Xray dataset:
https://github.com/ieee8023/covid-chestxray-dataset

Dataset was divided into 2 classes: COVID-19 and Other (Pneumonia Viral,Pneumonia bacterial and normal)

![Sample dataset](https://github.com/mayukhsil/DSND-Project-CRISP-DM-/blob/master/sample_images.JPG)

## Model Statistics and Accuracy
VGG16 and InceptionV3 model were utilized as base models (InceptionV3 was finally used), the layers were freezed and on top of it some more layers were added. The model was trained on 318 samples of data and tested on 48 samples. The testing accuracy currently reported is 95%.

### ROC Curve
![ROC curve of model](https://github.com/mayukhsil/DSND-Project-CRISP-DM-/blob/master/covid-roc.png)

### Classification Report: F1 Score, Precision, Recall
![Classification Report](https://github.com/mayukhsil/DSND-Project-CRISP-DM-/blob/master/cls_report.JPG)

### Confusion Matrix
[20 1]

[1 26]

![Confusion matrix](https://github.com/mayukhsil/DSND-Project-CRISP-DM-/blob/master/cmatrix.JPG)

# Result<a name="results"></a>
## Here is the the result of model on one of the samples:

![X-Ray of COVID-19 Positive patient](https://github.com/mayukhsil/DSND-Project-CRISP-DM-/blob/master/covid-19.JPG)
