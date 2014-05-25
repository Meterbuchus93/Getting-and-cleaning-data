Getting-and-cleaning-data
=========================
Begin by downloading data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
Then extract into the top level of the repository. then run using the command below which will apply analysis.

    Rscript run_analysis.R

The result will be two .csv files:

* measurements_mean_std.txt containing only the mean and standard deviation for each measurement
* activity_subject_means.txt containing the averages of the mean and the standard deviation per unique (activity, subject) pair

Refer to CodeBook.md for description of the extraction process and the columns in the two files.
