BALANCING

After preprocessing the dataset will be imbalanced towards one or more classes this inbalance must be dealt with using different techniques, this notebook uses stratify parameter of sklearn train_test_split to balance both test and train datasets on equal fraction of classes.

FEATURE EXTRACTION

Extracting features from audio sample is a task of its on, so using 3rd parties libraries help out a lot, here Librosa is used to extract three most important features namely MFCC, CHROMA STFT and MEL SPECTROGRAM

MODELING

Each feature is an matrix of frequencies which is treated as an heatmap of frequencies and passed through different model paths for specific training and then concatenated for general optimisation and classification. The model is Keras Function API Convotional Model with BatchNormalization and ReLU activation.
