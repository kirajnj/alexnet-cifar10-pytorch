# AlexNet for CIFAR-10

Implementation of the classic AlexNet architecture in PyTorch for image classification
on the CIFAR-10 dataset. The network:
- consists of five convolutional layers and three fully connected layers;
- accepts RGB images as input.

## Dataset
[CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)

## Workflow
- Data — CIFAR-10 loading, augmentation (flip, rotation, affine), normalization to [-1, 1]
- Model — AlexNetRGB: 5 conv layers + 3 FC layers + Dropout; ~611K parameters
- Training — Adam (lr=0.001), CrossEntropyLoss, batch size 64, 20 epochs
- Evaluation — classification_report, confusion matrix, error visualization
- Results — 78.97% test accuracy; no signs of overfitting
- Conclusion — stable CIFAR-10 classification; best classes: automobile, truck, ship, frog; weaker classes: cat↔dog, bird↔deer

## Training
<img width="1114" height="436" alt="training_curve" src="https://github.com/user-attachments/assets/680b2b06-f7fa-4d15-aae8-2fb3c4be8366" />

## Confusion matrix
<img width="1096" height="963" alt="confusion_matrix" src="https://github.com/user-attachments/assets/38e53034-1d69-4829-9568-a695dbd39509" />
