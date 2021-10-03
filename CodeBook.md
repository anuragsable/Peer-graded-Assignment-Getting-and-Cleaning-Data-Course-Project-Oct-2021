## Getting and Cleaning Data - peer assessment project


## Data Transformation Steps

1. Merging the training and the test sets to create one data set.
2. Extracting only the measurements on the mean and standard deviation for each measurement. 
3. Using descriptive activity names to name the activities in the data set
4. Appropriately labeling the data set with descriptive activity names. 
5. Creating a second, independent tidy data set with the average of each variable for each activity and each subject. 

## About R script
File with R code "run_analysis.R" performs the required operation to extract the final data set

## About variables:   

Following variables contains data downloaded from the downloaded files. </br>

FeaturesTest  	X_test </br>
FeaturesTrain 	X_train </br>
ActivityTest  	Y_test </br>
ActivityTrain 	Y_train </br>
SubjectTrain 	subject_train </br>
SubjectTest  	subject_test.txt </br>

Features, Activity and Subject datasets are used and merged to do the further analysis from the downloaed datasets</br>
Features <- rbind(FeaturesTrain, FeaturesTest)</br>
Activity <- rbind(ActivityTrain, ActivityTest)</br>
Subject  <- rbind(SubjectTrain, SubjectTest)</br>

###combine data to get one dataset</br>
Combine <- cbind(Subject, Activity)</br>
Data <- cbind(Features, Combine)</br>

##Subset "Data" with only units that have "mean" and "std" in the name</br>
DataSub <- Data %>% select(Subject, Activity, contains("mean"), contains("std"))</br>

##create final dataset with the means for each variable and subject</br>
FinalData</br>
