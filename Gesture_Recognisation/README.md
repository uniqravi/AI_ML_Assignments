# Gestures Recognisation System By DNN + RNN

### Introduction

Gestures Recognisation System By Deep Neural Network & Recurrent Neural Network

### Problem Statement

Imagine A Electronics Company wants to manufacture state-of-the-art smart televisions. Company want to add cool feature for the smart TV that can recognize five different gestures performed by the user, allowing control of the TV without a remote.

The TV's webcam continuously monitors gestures, each corresponding to a specific command:

- Thumbs up: Increase the volume
- Thumbs down: Decrease the volume
- Left swipe: Jump backward 10 seconds
- Right swipe: Jump forward 10 seconds
- Stop: Pause the movie

### Dataset Details:
The training data consists of a few hundred videos categorised into one of the five classes. 

Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use. 

### Solution/Approaches:

I build CNN + RNN architecture and then I perfomred follwoing set of experiment and result 

### Experiment Result:
| Experiment                                           | Validation Accuracy (%) | Training Accuracy (%) |
|------------------------------------------------------|-------------------------|------------------------|
| SimpleCnn_Plus_Rnn_with_15Frame                      | 93.00                   | 98.49                  |
| TransferLearning_ResNetCnn_Rnn_with_15Frame          | 100.00                  | 83.00                  |
| Basic_Conv3D_15_Frames                               | 99.49                   | 96.00                  |
| ResNetBlock_Conv3D_15_Frames                         | 93.96                   | 92.00                  |
| ResNetBlock_Conv3D_15_Frames_with_Augmentation       | 74.00                   | 71.00                  |

### Conclusion:

- Each model was trained for 30 epochs. Initially, the optimal learning rate for each model architecture was determined. Then, using the plots, we assessed whether learning rate decay was necessary. Some curves showed zigzag patterns at lower learning rates, indicating the need to reduce the learning rate as the model approaches the minimum.
- The best validation accuracy achieved was 96%, obtained from the ResNetBlock_Conv3D_15_Frames model. The ResNet block helped mitigate the gradient vanishing problem, keeping both validation and training accuracies close together.
- The validation and training accuracies of the SimpleCnn_Plus_Rnn model followed each other closely, as seen in the model history curves.
- Other than SimpleCnn_Plus_Rnn and ResNetBlock_Conv3D_15_Frames, the validation accuracies of the models exhibited zigzag patterns.
- I observed that networks with a high number of parameters tend to overfit, so I aimed to keep the models as simple as possible.
- For example, the Transfer Learning model showed trends of overfitting.
- Augmentation did not work well in this problem, possibly because it distorted the image sequence, causing confusion.
- Applying different augmentations to each image of a single frame might not be the right approach.
