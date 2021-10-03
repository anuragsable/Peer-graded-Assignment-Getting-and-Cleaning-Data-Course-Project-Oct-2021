The purpose of this project is to create clean dataset from measurements described in "Human Activity Recognition Using Smartphones Dataset".

**Preparation**

Unzip the provided zip file ( https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip  ) to data/external directory. 

**Goal**

As per the rquirement, we need to merge the training and the test sets to create one data set.Extracts only the measurements on the mean and standard deviation for each measurement. 
And the second dataset shall be independent tidy data set with the average of each variable for each activity and each subject.

**Executing the Project**

To start the project, simply execute run_analysis.R. 

The combined data is stored in Combine variable
The final data is exported into FinalData.txt file.
CodeBook.md describes about variables and other details.

**Implementation**

Structure of the project
The root (or base or main directory) directory contains 4 files :

README.md explains everything needed to use the project.</br>
CodeBook.md explains the variables and datasets used in the project.</br>
run_analysis.R is the main R script to excute to create the resulting datasets.</br>
FinalData.txt is the final dataset created by the project.
