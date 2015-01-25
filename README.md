# Introduction

The run_analysis.R analysis the original data for the peer assignment by the following way:

# 0. prepare the data files
Download and unzip the data if it is not ready in the working directory i

# 1. Merges the training and the test sets to create one data set.
    according to the readme.txt in dataset, these files are processing:
    - 'train/X_train.txt': Training set.
    - 'train/y_train.txt': Training labels.
    - 'test/X_test.txt': Test set.
    - 'test/y_test.txt': Test labels.

Get column names from the dataset feature.txt 
Pre-process the fixed-width file contains leading whitespace and double whitespace separator
and then merge the datas of train+test.
# 2 Extracts only the measurements on the mean and standard deviation for each measurement.
with the data which column name contains "mean" and "std"

# 3. Uses descriptive activity names to name the activities in the data set
  It is done by apply make.names to the data from feature.txt

# 4. Appropriately labels the data set with descriptive variable names. 
 Create an ID column to keep the order of labels and merge original label with feature description

# 5. From the data set in step 4, creates a second,
   independent tidy data set with the average of 
   each variable for each activity and each subject.
   the tidy data is saved in avg_act_subject.txt
   
The CodeBook.md keep the column name from feature.txt and the column V1(subject) and the column label(activity label).

