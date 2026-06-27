# Cell Type Prediction

For the Cell Type Prediction challenge we were given 13759 96x96 RGB images of blood cells, each one labeled as one of 8 possible classes.

We both tried building a CNN from scratch, both imported pre-trained models from Keras Applications.

We had to deal with:
- outliers in the dataset
- class imbalance in the dataset
- necessity for data augmentation (the challenge was revealed to strtongly be about it)

Our best result on the test set which was not available to us was obtained with the EfficientNetV2L model, with a 89% accuracy.

A better explanation of the work we did can be found [here](report_prediction.pdf)

The notebooks are organized as follows:

- [1_CustomCNN.ipynb](1_CustomCNN.ipynb): CNN built from scratch
- [2_TransferLearningFineTuning.ipynb](2_TransferLearningFineTuning.ipynb): transfer learning and fine-tuning experiments
- [3_FineTuningGradualUnfreezing.ipynb](3_FineTuningGradualUnfreezing.ipynb): gradual unfreezing strategy
