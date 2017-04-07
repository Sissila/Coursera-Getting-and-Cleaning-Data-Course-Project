# Introduction

The script `run_analysis.R`performs the 5 steps described in the course project's definition:

* We merge the training and the test sets to create one data set using `rbind()` and we address the files having same number of columns and referring to same entities.
* We extract only the measurements on the mean and standard deviation for each measurement. After extracting the columns, we give them correct names that are taken from `features.txt`.
* We use descriptive activity names to name the activities in the data set using the names and the IDs existing in `activity_labels.txt`.
* We appropriately label the data set with descriptive variable names.
* From the data set in step 4, we create a second, independent tidy data set with the average of each variable for each activity and each subject.

# Variables

* `x_train`, `y_train`, `x_test`, `y_test`, `subject_train` and `subject_test` contain the data from the downloaded files.
* `x_data`, `y_data` and `subject_data` merge the previous datasets to further analysis.
* `features` contains the correct names for the `x_data` dataset.
*  A similar approach is taken with activity names through the `activities` variable.
* `all_data` merges `x_data`, `y_data` and `subject_data` in a big dataset.
*  Finally, `averages_data` contains the relevant averages which will be later stored in a `.txt` file. 
