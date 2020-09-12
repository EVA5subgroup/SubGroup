# Week-7 Requirements

1. change the code such that it uses GPU
2. change the architecture to C1C2C3C40 (basically 3 MPs)
3. total RF must be more than 44
4. one of the layers must use Depthwise Separable Convolution
5. one of the layers must use Dilated Convolution
6. use GAP (compulsory):- add FC after GAP to target #of classes (optional)
7. achieve 80% accuracy, as many epochs as you want. Total Params to be less than 1M.

## Results - 
1. Total Parameters - 330538
2. Final Receptive Field - 108

### Test Accuracy Vs Epoch
![TestAccuracy Vs Epoch](https://github.com/vamsigp/EVA5/blob/master/week-7/Trails-2/val_test%20accuracy_change.png)

### TestLoss Vs Epoch
![Test Loss Vs Epoch](https://github.com/vamsigp/EVA5/blob/master/week-7/Trails-2/val_test%20losses_change.png)

### Misclassified Images
![Misclassified Images](https://github.com/vamsigp/EVA5/blob/master/week-7/Trails-2/misclassified_images.png)

##

## Learning - 
1. Could write Framework in a more better way

    a. Need to apply Scheduler
    
    b. Need to modularize better
  
2. Could have applied Learning Rate Scheduler after 25 Epochs
