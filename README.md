# audio_classficiation_model

# data used
1. Data used are .wav files of length 1sec each for 10 classes. 
2. Audio is converted into numerical format and MFCC values had been generated and saved in data.json file

# train, test, validation sets
1. Since data is huge, I have divided it into train, test and validation using custom metjods prepare_dataset()

# model architecture
1. A CNN model with 3 hidden layers along with ReLU activation function is used to capture the patterns in data.
2. 62 neurons in 1st hidden layes, 32 neurons units in 2nd, 3rd hidden layers.
3. Maxpooling ater each layer
4. Finally all values are flatened and passed into a dense layer with softmax actvation function to do classfication. 
5. For hyper paramater tuning: Used adam, rmsprop optimisers and also early stopping, and epoch, batchsize values.


# metrics
1. Accuracy of Model is 96% on train and 93% on test(data on which model is not adjusted) using the cnn model. 

