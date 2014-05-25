Data Source:
https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip,
Description:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones


## Procedure to extract data:

* read X, y and subject data for both train and test datasets
* merge X, y and subject data for both train and test datasets
* read in features descriptions
* set descriptive names for all columns in merged X, y and subject data
* select features containing measurements on the mean and standard deviation
* read in activity descriptions
* join activity dataset with descriptive labels
* join measurements dataset with activity labels
* write this first result data set to csv file "measurements_mean_std.txt"
* join previous result data set with subject ids
* summarize means per unique (activity, subject) pair
* write this second result data set to csv file "activity_subject_means.txt"


## The meaning of the columns in measurements_mean_std.txt is as follows:

column   | description
---------|------------------------------
activity | descriptive label of activity

All the other columns list the measurements as described in the
features_info.txt file in the original raw data set.


## The meaning of the columns in activity_subject_means.txt is as follows:

column   | description
---------|------------------------------
activity | descriptive label of activity
subject  | test subject id

All the other columns list the measurements as described in the
features_info.txt file in the original raw data set.

Note: Only data for the activities that subjects actually performed is listed.
