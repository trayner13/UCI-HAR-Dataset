Getting and Cleaning Data: Coursera Course Project
=========================================

Introduction
------------
This repository was created as part of the requirements for completion of the Coursera course "Getting and Cleaning data" within the Data Science specialization.

About the raw data
------------------

The features (561 of them) are unlabeled and can be found in the x_test.txt. 
The activity labels are in the y_test.txt file.
The test subjects are in the subject_test.txt file.

The training dataset is set up in the same fashion, but "test" is replaced with "train".

About the script and the tidy dataset
-------------------------------------
The script called run_analysis.R merges the test and training sets together.
Prerequisites for this script:

1. the UCI HAR Dataset must be extracted and..
2. the UCI HAR Dataset must be availble in a directory called "UCI HAR Dataset"
3. your working directory must be set to ".../UCI HAR Dataset"

After testing and training datasets are merged, labels are added. Only columns that have to do with mean and standard deviation are kept.

The script will then create a tidy data set containing the means of all the columns per test subject and per activity.
This tidy dataset will be written to a tab-delimited file called "data_set_with_the_averages.txt", which can also be found in this repository.

About the Code Book
-------------------
The CodeBook.md file explains the transformations performed and the resulting data and variables.
