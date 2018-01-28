# Human_Activity_Classification_Using_Deep_Nets
Classify human activity using accelerometer and gyroscope data from mobile phone.

Input Data:
1. Triaxial acceleration from the accelerometer (total acceleration) and the estimated body acceleration.
2. Triaxial Angular velocity from the gyroscope.
3. A 561-feature vector with time and frequency domain variables.
4. Activity Label
5. An identifier of the subject who carried out the experiment.

Output classes:
WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING

Data preprocessing:
- Features are normalized and bounded within [-1,1].
- Each feature vector is a row on the text file.
- The units used for the accelerations (total and body) are 'g's (gravity of earth -> 9.80665 m/seg2).
- The gyroscope units are rad/seg.

Dataset courtesy:
https://archive.ics.uci.edu/ml/machine-learning-databases/00240/

Model Structure:
