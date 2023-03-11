# HAD-ANC: A Hybrid System Comprising an Adaptive Filter and Deep Neural Networks for Active Noise Control ANC system  
  
## Model for HAD-ANC
  
## Subscription of development set preparation  
### 1. Download 16 kHz noise signal
We used DEMAND https://zenodo.org/record/1227121#.ZAxCu3ZByUk
  
and MS-SNSD https://github.com/microsoft/MS-SNSD.
  
Note that exclude labeled as "babble" signal in [noise train](https://github.com/microsoft/MS-SNSD/tree/master/noise_train) and [noise_test](https://github.com/microsoft/MS-SNSD/tree/master/noise_test) of MS-SNSD.

### 2. Creating development set
Split into six-second all signals audio clips.
Normalize all 15639 clips.

### 3. Creating validation set
### 4. Creating test set
