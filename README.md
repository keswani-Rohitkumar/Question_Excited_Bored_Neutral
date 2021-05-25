Intonation Prediction

In this project I have built a model that predicts the intonation of a short audio segment.
The audio dataset was prepared by the batch of MSc Big Data Science at QMUL.

The trainingMLEND.csv consits of 20k rows and 4 columns. Each row corresponds to one of the items in our dataset, and each item is described by four attributes.
1) File ID (audio file)
2) Numeral
3) Participand ID
4) Intonation

Here I have extracted many features from the audio signal namely 
1) Power
2) Pitch mean
3) Pitch standard deviation
4) Fraction of voiced region
using librosa library.

I build 6 models which are

1) SVM
2) RandomForest
3) KNN
4) Naive Bayes
5) Logistic Regression
6) MuliLayer Perceptron Classifier

I build these models and trained them on hyperparameters, tuning them with the help of GridSearch CV. I build these models for both normalised predictors and without normalised also and with extra features such as mfcc and experimented them.

Finally, Getting the highest Accuracy on the SVM model with the accuracy of 53.5% on the validation data with normalised predictors.
