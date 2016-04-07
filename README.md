# Getting and Cleaning Data - Course Project

This is the repo for the submission of the course project for Coursera's Getting and Cleaning Data course.  It includes:
<ul>
<li><code>run_analysis.R</code> - scripts needed to create desired tidy data set</li>
<li><code>codebook.MD</code> - information on varialbes, data and transformations</li>
<li><code>TidyData.txt</code> - resulting data set from <code>run_analysis.R</code></li>
</ul>

##Modifications to <code>run_analysis.R</code>
Note that lines 1 and 19 will need to be altered to set the path of the working directory.  

##Summary of <code>run_analysis.R</code>
<ol>
<li>Merges the training and the test sets to create one data set.</li>
<li>Extracts only the measurements on the mean and standard deviation for each measurement.</li>
<li>Uses descriptive activity names to name the activities in the data set</li>
<li>Appropriately labels the data set with descriptive variable names.</li>
<li>From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.</li>
</ol>
