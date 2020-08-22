# Coding Drill

0. Base Model
   - [EVA5_WK_5_Base](./week-5/EVA5_WK_5_Base.ipynb)

   Model is based on this class file

1. Iteration 1

    - [EVA5_WK_5_1](./week-5/EVA5_WK_5_1.ipynb)
    1. Target

          Get setup right.
          Target decent accuracy
          setup baseline model
          Run training for 15 epoch

      2. Result

          Params - 7432
          Best Train Accuracy - 98.74 @Epoch 14
          Best Test Accuracy - 98.60% @ Epoch 13

      3. Analysis

          Able to reduce the number of parameters below the desired level
          Model is training properly - as both training and testing accuracries are improving till last epoch.
          Model hasnt reach plateau, is capable if pushed further


2. Iteration 2

    - [EVA5_WK_5_2](./week-5/EVA5_WK_5_2.ipynb)
    1. Target

        Increase Accuracy

    2. Result

        Params - 7758
        Best Test accuracy - 99.35 at Epoch - 13
        Best Train accuracy - 99.44 at Epoch - 14

    3. Analysis

        Able to increase accuracy upto 99.3%
        After adding Batch Normalization, Model was overfitting
        Added Dropout(Regularization) to counter overfitting
        Modified model to add more convolution layers and remove second maxpooling layer
        Model not overfitting - but observed test accuracy oscillations


3. Iteration 3

    - [EVA5_WK_5_3](./week-5/EVA5_WK_5_3.ipynb)
    1. Target

        Increase Accuarcy
        Add Image Augmentation(Image Transformation)
        Add model capacity by addding a convolution layer after GAP

    2. Result

        Params - 7758
        Best Test accuracy - 99.32 at Epoch - 6
        Best Train accuracy - 99.13 at Epoch - 14

    3. Analysis

        Able to increase accuracy upto 99.32%
        Able to reach the top accuracy at Epoch 6, where as in previous model able to reach at 13 ### TODO - Need to reduce learning rate to achieve the desired accuracy


4. Iteration 4

    - [EVA5_WK_5_4](./week-5/EVA5_WK_5_4.ipynb)

    1. Target

         Reach target Accuracy
         Model Accuracy should be consistent
         Add Learning rate scheduler

    2. Result

        Params - 7758
        Best Test accuracy - 99.51 at Epoch - 8
        Best Train accuracy - 99.20 at Epoch - 14

    3. Analysis

        Able to reach desired accuracy - 99.4%
        Accuracy is consistent, from Epoch 7 accuracy consistently above 99.4
        As observed previously, applying LR resulted in deriving desired accuracy.
