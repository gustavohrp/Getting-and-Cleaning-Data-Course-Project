#Code Book
##This document describes the code in run_analysis script. The code is devided by comments in multiple categories:

1. Chicking the availability of data and packages
2. Reading data
3. Merging data
4. Adding descriptive names and labels
5. Subsetting only features connected to mean and standard deviation
6. Getting average for all activities and subjects
7. Writing new data to file

##Checking availability of data and packages

Script assumes that UCI HAR Dataset is placed in your working directory. Dplyr package is required for this scipt

##Reading data

Test and training data is read to R variables using read.table function

##Merging data

Test and Training data is merged together in one variable using cbind and rbind commands

##Adding descriptive names and labels

To set appropriate names for each features features.txt file was used. It contains names for all features. To set names for activity type file activity_labels.txt was used.

##Subsetting only features connected to mean and standard deviation

Using select R command, data was changed to data that has only columns connected to mean or std.

##Getting average for all activities and subjects

Using Ddply function we created a new data frame, that contains averages of all columns of data, divided by activity and subject

##Writing new data to file

We wrote new data set to file using write.table function.

##Identifiers

*subject - The ID of the test subject
*activity - The type of activity performed when the corresponding measurements were taken

##Measurements

*tBodyAccMeanX
*tBodyAccMeanY
*tBodyAccMeanZ
*tBodyAccStdX
*tBodyAccStdY
*tBodyAccStdZ
*tGravityAccMeanX
*tGravityAccMeanY
*tGravityAccMeanZ
*tGravityAccStdX
*tGravityAccStdY
*tGravityAccStdZ
*tBodyAccJerkMeanX
*tBodyAccJerkMeanY
*tBodyAccJerkMeanZ
*tBodyAccJerkStdX
*tBodyAccJerkStdY
*tBodyAccJerkStdZ
*tBodyGyroMeanX
*tBodyGyroMeanY
*tBodyGyroMeanZ
*tBodyGyroStdX
*tBodyGyroStdY
*tBodyGyroStdZ
*tBodyGyroJerkMeanX
*tBodyGyroJerkMeanY
*tBodyGyroJerkMeanZ
*tBodyGyroJerkStdX
*tBodyGyroJerkStdY
*tBodyGyroJerkStdZ
*tBodyAccMagMean
*tBodyAccMagStd
*tGravityAccMagMean
*tGravityAccMagStd
*tBodyAccJerkMagMean
*tBodyAccJerkMagStd
*tBodyGyroMagMean
*tBodyGyroMagStd
*tBodyGyroJerkMagMean
*tBodyGyroJerkMagStd
*fBodyAccMeanX
*fBodyAccMeanY
*fBodyAccMeanZ
*fBodyAccStdX
*fBodyAccStdY
*fBodyAccStdZ
*fBodyAccMeanFreqX
*fBodyAccMeanFreqY
*fBodyAccMeanFreqZ
*fBodyAccJerkMeanX
*fBodyAccJerkMeanY
*fBodyAccJerkMeanZ
*fBodyAccJerkStdX
*fBodyAccJerkStdY
*fBodyAccJerkStdZ
*fBodyAccJerkMeanFreqX
*fBodyAccJerkMeanFreqY
*fBodyAccJerkMeanFreqZ
*fBodyGyroMeanX
*fBodyGyroMeanY
*fBodyGyroMeanZ
*fBodyGyroStdX
*fBodyGyroStdY
*fBodyGyroStdZ
*fBodyGyroMeanFreqX
*fBodyGyroMeanFreqY
*fBodyGyroMeanFreqZ
*fBodyAccMagMean
*fBodyAccMagStd
*fBodyAccMagMeanFreq
*fBodyBodyAccJerkMagMean
*fBodyBodyAccJerkMagStd
*fBodyBodyAccJerkMagMeanFreq
*fBodyBodyGyroMagMean
*fBodyBodyGyroMagStd
*fBodyBodyGyroMagMeanFreq
*fBodyBodyGyroJerkMagMean
*fBodyBodyGyroJerkMagStd
*fBodyBodyGyroJerkMagMeanFreq

##Activity Labels
*WALKING (value 1): subject was walking during the test
*WALKING_UPSTAIRS (value 2): subject was walking up a staircase during the test
*WALKING_DOWNSTAIRS (value 3): subject was walking down a staircase during the test
*SITTING (value 4): subject was sitting during the test
*STANDING (value 5): subject was standing during the test
*LAYING (value 6): subject was laying down during the test
