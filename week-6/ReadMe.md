# Assignment 6

1. with L1 + BN
2. with L2 + BN
3. with L1 and L2 with BN
4. with GBN
5. with L1 and L2 with GBN


some observations - 
1. Switching from L2 to L1 regularization dramatically reduces the delta between test loss and training loss.
2. Switching from L2 to L1 regularization dampens all of the learned weights.
3. Increasing the L1 regularization rate generally dampens the learned weights; however, if the regularization rate goes too high, the model can't converge and losses are very high.

|  | Max Accuracy at Epoch | Accuracy at last Epoch | Total Misclassifications |
| -- | -- | -- | -- |
|Batch Normalization|99.47 @ 15|99.4|60|
|Batch Normalization + L1 Reg | 99.46 @ 8,12,14| 99.44 | 56 |
|Batch Normalization + L1 + L2 Reg | 99.45 @ 24 | 99.45 | 55 |
|Ghost Batch Normalization | 99.52 @ 22 | 99.47 | 53 |
|Ghost Batch Normalization + L1 + L2 Reg | 99.44 @ 17 | 99.41 | 59 |

## Test Accuracy Vs Epoch
![Graph for Test Acc Vs Epoch](https://github.com/vamsigp/EVA5/blob/master/week-6/images/acc%20vs%20epochs.png)


## Test Loss Vs Epoch
![Graph for Test Loss Vs Epoch](https://github.com/vamsigp/EVA5/blob/master/week-6/images/loss%20vs%20epochs.png)

## Misclassifications for Ghost-BatchNormalization Model
![Misclassification_image_GBN](https://github.com/vamsigp/EVA5/blob/master/week-6/images/gbn/misclassification.png)
