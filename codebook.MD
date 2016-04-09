#Codebook for Getting and Cleaning Data Course Project

Information about the variables, data and transformations used in the Getting and Cleaning Data course project.

Source data can be found <a href="http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones" target="blank">here</a>.

<h3>Data Set Information:</h3>

The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, we captured 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data. 

The sensor signals (accelerometer and gyroscope) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a vector of features was obtained by calculating variables from the time and frequency domain.

<h3>Attribute Information:</h3>

For each record in the dataset it is provided: 
<ul>
<li>Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.</li>
<li>Triaxial Angular velocity from the gyroscope.</li>
<li>A 561-feature vector with time and frequency domain variables.</li>
<li>Its activity label.</li>
<li>An identifier of the subject who carried out the experiment.</li>
</ul>

<h3> Overview of <code>run_analysis.R:</code></h3>
<ol>
<li>Set the working directory and read the following files into tables: <code>features.txt</code>, <code>activity_labels.txt</code>, <code>subject_train.txt</code>, <code>x_train.txt</code>, <code>y_train.txt</code>, <code>subject_test.txt</code>, <code>x_test.txt</code> and <code>y_test.txt</code>.  Assign column names and merge the data into a single data set.</li>
<li>Create a logcal vector that contains TRUE values for the ID, mean and standard deviation columns and FALSE values for the others. Subset this data to keep only the necessary columns.</li>
<li>Merge data subset with the activityType table to inlude the descriptive activity names.</li>
<li>Provide descriptive lables using the gsub funtion.</li>
<li>Create a <code>.txt</code> file that contains only a data set with the average of each variable for each activity and subject.</li>
</ol>

</ol>
