## Human Activity Recognition Using Smartphones Dataset
## Version 1.0
### Variables used on the feature vector 
* The __features__ selected for this database come from the _accelerometer_ and _gyroscope_ 3-axial raw signals tAcc-XYZ and tGyro-XYZ. These time domain signals (prefix 't' to denote time) were captured at a constant rate of 50 Hz. Then they were filtered using a median filter and a 3rd order low pass Butterworth filter with a corner frequency of 20 Hz to remove noise. Similarly, the acceleration signal was then separated into body and gravity acceleration signals (tBodyAcc-XYZ and tGravityAcc-XYZ) using another low pass Butterworth filter with a corner frequency of 0.3 Hz.
* Subsequently, the _body linear acceleration_ and _angular velocity_ were derived in time to obtain Jerk signals (tBodyAccJerk-XYZ and tBodyGyroJerk-XYZ). Also the magnitude of these three-dimensional signals were calculated using the Euclidean norm (tBodyAccMag, tGravityAccMag, tBodyAccJerkMag, tBodyGyroMag, tBodyGyroJerkMag).
* Finally a _Fast Fourier Transform (FFT)_ was applied to some of these signals producing fBodyAcc-XYZ, fBodyAccJerk-XYZ, fBodyGyro-XYZ, fBodyAccJerkMag, fBodyGyroMag, fBodyGyroJerkMag. (Note the 'f' to indicate frequency domain signals).
* These _signals_ were used to estimate variables of the feature vector for each pattern:  
'-XYZ' is used to denote 3-axial signals in the X, Y and Z directions.
    * tBodyAcc-XYZ
    * tGravityAcc-XYZ
    * tBodyAccJerk-XYZ
    * tBodyGyro-XYZ
    * tBodyGyroJerk-XYZ
    * tBodyAccMag
    * tGravityAccMag
    * tBodyAccJerkMag
    * tBodyGyroMag
    * tBodyGyroJerkMag
    * fBodyAcc-XYZ
    * fBodyAccJerk-XYZ
    * fBodyGyro-XYZ
    * fBodyAccMag
    * fBodyAccJerkMag
    * fBodyGyroMag
    * fBodyGyroJerkMag
    
* The set of variables that were __estimated__ from these signals are:
    * mean(): Mean value
    * std(): Standard deviation
    * mad(): Median absolute deviation 
    * max(): Largest value in array
    * min(): Smallest value in array
    * sma(): Signal magnitude area
    * energy(): Energy measure. Sum of the squares divided by the number of values. 
    * iqr(): Interquartile range 
    * entropy(): Signal entropy
    * arCoeff(): Autorregresion coefficients with Burg order equal to 4
    * correlation(): correlation coefficient between two signals
    * maxInds(): index of the frequency component with largest magnitude
    * meanFreq(): Weighted average of the frequency components to obtain a mean frequency
    * skewness(): skewness of the frequency domain signal 
    * kurtosis(): kurtosis of the frequency domain signal 
    * bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.
    * angle(): Angle between to vectors.
* __Additional vectors__ obtained by averaging the signals in a signal window sample. These are used on the _angle()_ variable:
    * gravityMean
    * tBodyAccMean
    * tBodyAccJerkMean
    * tBodyGyroMean
    * tBodyGyroJerkMean

#### Notes:
* Features are normalized and bounded within [-1,1].
* Each feature vector is a row on the text file.

### Additional information:
#### Acknowledgement
* Jorge L. Reyes-Ortiz, Davide Anguita, Alessandro Ghio, Luca Oneto.
* Smartlab - Non Linear Complex Systems Laboratory
DITEN - University degli Studi di Genova.
Via Opera Pia 11A, I-16145, Genoa, Italy.
* [activityrecognition@smartlab.ws](activityrecognition@smartlab.ws)
* [www.smartlab.ws](www.smartlab.ws)

#### How the Experiment was Conducted
* The __experiments__ have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (__Samsung Galaxy S II__) on the waist. Using its embedded accelerometer and gyroscope, 3-axial linear acceleration and 3-axial angular velocity was captured at a constant rate of 50Hz. The experiments have been video-recorded to label the data manually. The obtained dataset has been randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.
* The sensor signals (__accelerometer and gyroscope__) were pre-processed by applying noise filters and then sampled in fixed-width sliding windows of 2.56 sec and 50% overlap (128 readings/window). The sensor acceleration signal, which has gravitational and body motion components, was separated using a Butterworth low-pass filter into body acceleration and gravity. The gravitational force is assumed to have only low frequency components, therefore a filter with 0.3 Hz cutoff frequency was used. From each window, a __vector of features__ was obtained by calculating variables from the time and frequency domain. 

#### For each record it is provided:
- Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
- Triaxial Angular velocity from the gyroscope. 
- A 561-feature vector with time and frequency domain variables. 
- Its activity label. 
- An identifier of the subject who carried out the experiment.

#### License:
- Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012
- This dataset is distributed __AS-IS__ and no responsibility implied or explicit can be addressed to the authors or their institutions for its use or misuse. _Any commercial use is prohibited_.
- Jorge L. Reyes-Ortiz, Alessandro Ghio, Luca Oneto, Davide Anguita. November 2012.
