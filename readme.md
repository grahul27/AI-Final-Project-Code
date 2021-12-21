# MM811 Final Project - Afib Detection

### Please find the instructions to run the code

#### Download the dataset from the drive link

https://drive.google.com/drive/folders/1X_JV5HvmzhNrgzqMBe7CsMqxHHO_ppCb?usp=sharing

Add the data file to the root folder of the project.

Dataset file is different for both 1D and 2D CNN, please change the file path in the files accordingly.

1. File 1D CNN Afib Detection.ipynb is implementation of 1D CNN to detect Afib. It is a 10 layer convolutional neural network with each layer having a pooling layer.
   To avoid bias in the model we 90% of data for training and 10% as test dataset.

We have Adam optimizer as our optimization function and binary-cross entropy as our loss function.
we have trained our model over 100 epochs with a batch size of 128.

2. File 2D CNN Afib Detection.ipynb is implementation of 2D CNN to detect Afib using physioNet Dataset by converting time series data into spectrograms.
   we have implemented a 24 layer convolutional neural network to train our dataset over 50 epochs of batch size 50 and temporal aggregation is achieved using Lambda layer. The model achieved accuracy of 74%.
