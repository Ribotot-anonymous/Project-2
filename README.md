# HAD-ANC: A Hybrid System Comprising an Adaptive Filter and Deep Neural Networks for Active Noise Control ANC system  
  
## Model for HAD-ANC
  
## Subscription of development set preparation  
### 1. Download 16 kHz noise signal
Download DEMAND https://zenodo.org/record/1227121#.ZAxCu3ZByUk
  
and MS-SNSD https://github.com/microsoft/MS-SNSD.
  
Note that exclude labeled as "babble" signal in [noise train](https://github.com/microsoft/MS-SNSD/tree/master/noise_train) and [noise_test](https://github.com/microsoft/MS-SNSD/tree/master/noise_test) of MS-SNSD.

### 2. Create development set
Split all signals into 6-second audio clips and index them in order.
  
Then normalize all 15639 clips.

### 3. Create validation set
Select the audio clips indexed by a multiple of 10 in the development set.
  
Multiply each of them by random numbers between 0.3 and 1.0.

### 4. Create train set
Once the validation sets consisting of 1,563 signals are created, the remaining audio clips from the development set compose the train set.
