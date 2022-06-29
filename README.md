# Modulation-Classification

## Problem statement

DeepSig Dataset: RadioML 2016.04C. (You can find the dataset in this <a href = "https://opendata.deepsig.io/datasets/2016.10/RML2016.10b.tar.bz2">link</a>)<br>
A synthetic dataset, generated with GNU Radio, consisting of 11 modulations. This 
is a variable-SNR dataset with moderate LO drift, light fading, and numerous 
different labeled SNR increments for use in measuring performance across different 
signal and noise power scenarios.<br>
Every sample is presented using two vectors (two channels) each of them has 128 elements.<br>
Please note: I've downloaded the data in my drive and mounted it in order to access it.

## Model

![Model](https://github.com/AmrMomtaz/Modulation-Classification/blob/main/images/model.png)<br>

This is the CNN model and I've replaced the final dense layer (consisting of 10 neurons) with LSTM layer.<br>
The data is splited into 70% for training/validation and 30% for testing. And 5% of the training and validation dataset for validation.<br>

Training performance:<br>
![Train](https://github.com/AmrMomtaz/Modulation-Classification/blob/main/images/tarining.png)

## Testing
