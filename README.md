# human_activity_classification
Feed forward neural network that classifies the current physical activity of the user using accelerometer and gyroscope data from mobile phone.

# Acheived accuarcy of ~96 after 1000 epochs.

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

Model Structure:
1. Input layer with 561 features
2. Second layer with 100 neuron and RELU
3. Third layer with 50 neuron and RELU
4. Bang, dropout of .5 to fire off 50% random neuron
5. Fourth layer with 25 neuron and RELU
6. Fifth layer with 10 neuron and RELU
7. Sixth layer with 5 neuron and RELU
8. Last layer with 6 classification with softmax function, since it is a multi-class classification. 



Dataset courtesy:
https://archive.ics.uci.edu/ml/machine-learning-databases/00240/
