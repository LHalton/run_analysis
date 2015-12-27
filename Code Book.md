# Overview
Source where data was obtained: http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 
Source of data used: https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 

# Process
R script called run_analysis.R that does the following:	
1. Merges the training and the test sets to create on data set.
2. Extracts only the measurements on the mean and standard deviation for each measurement.
3. Uses descriptive acticity names to name the activities in the data set.
4. Appropriately labels the data set with descriptive variable names.
5. From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

# Variables
activity_labels: Reads "activity_labels.txt" file 
features: Loads data column names
extract_features: Measures the mean and standard deviation for each measurement.
X_test: loads the "X_test" and "y_test" data.y_test <- read.table("~/UCI HAR Dataset/test/y_test.txt")
subject_test: Reads "subject_test.txt" file.
test_data: Label of the step that binds the data.
X_train: Loads the "X_train.txt" file. 
y_train: Loads the "y_train.txt" file. 
subject_train: Reads the "subject_train.txt" file.
train_data: Label of the step that binds the data.

#Ouput
tidy_data.txt is the name of the txt output.
