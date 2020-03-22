Gender Recognition by Voice and Speech Analysis

This database was created to identify a voice as male or female, based upon acoustic properties of the voice and speech. The dataset consists of 3,168 recorded voice samples, collected from male and female speakers. The voice samples are pre-processed by acoustic analysis in R using the seewave and tuneR packages, with an analyzed frequency range of 0hz-280hz (human vocal range).
To access this dataset click on the link below

https://www.kaggle.com/primaryobjects/voicegender

The Dataset

The following acoustic properties of each voice are measured and included within the CSV:

meanfreq: mean frequency (in kHz)

sd: standard deviation of frequency

median: median frequency (in kHz)

Q25: first quantile (in kHz)

Q75: third quantile (in kHz)

IQR: interquantile range (in kHz)

skew: skewness (see note in specprop description)

kurt: kurtosis (see note in specprop description)

sp.ent: spectral entropy

sfm: spectral flatness

mode: mode frequency

centroid: frequency centroid (see specprop)

peakf: peak frequency (frequency with highest energy)

meanfun: average of fundamental frequency measured across acoustic signal

minfun: minimum fundamental frequency measured across acoustic signal

maxfun: maximum fundamental frequency measured across acoustic signal

meandom: average of dominant frequency measured across acoustic signal

mindom: minimum of dominant frequency measured across acoustic signal

maxdom: maximum of dominant frequency measured across acoustic signal

dfrange: range of dominant frequency measured across acoustic signal

modindx: modulation index. Calculated as the accumulated absolute difference between adjacent measurements of fundamental frequencies divided by the frequency range

label: male or female


The dataset contains 3168 rows and 21 columns of data. Each column except the last one, has a numerical value which represents an acoustic property which collectively determine the gender of the voice.
The last column contains categorical data i.e two classes of data, Male and female.Therefore it is a binary classification dataset.


Models used for training and results:

Since it is a classification dataset, the models used are:

1. Neural networks

Training accuracy:98.55%

Validation accuracy:98.42%

2.Logistic regression

Training accuracy:95.30%

Test accuracy:95.74%

3.KNN

Accuracy:96.84%


Instructions to follow while going through the notebooks:

1.Since I have written the code on google colab, you can upload it and execute it on Google Colab in the following order

  a) The Data Visualization.ipynb has different visualisations to understand the data
  
  b) The Gender recognistion using Logistic regression(2 variables).ipynb notebook for logistic regression
  
  c) Gender recognition using neural networks.ipynb notebook has code to implement neural networks
  
  d) Gender recg using KNN.ipynb notebook had code for implementing KNN

You can download the .ipynb files on your system using Download or Clone button 



