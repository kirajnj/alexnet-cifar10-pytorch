# AlexNet for CIFAR-10 

An implementation of AlexNet in PyTorch for image classification using the CIFAR-10 dataset.

## Dataset
[CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) 

## Results
- **Test accuracy: 78.97%**
- 20 epochs, Adam (lr=0.001), CrossEntropyLoss, batch size 64
- Data augmentation: RandomHorizontalFlip, RandomRotation, RandomAffine
- Architecture: 5 conv + 3 FC layers, ReLU, MaxPool after Conv 1/2/5, Dropout 0.5 

## Training
<img width="1114" height="436" alt="training_curve" src="https://github.com/user-attachments/assets/680b2b06-f7fa-4d15-aae8-2fb3c4be8366" />

## Confusion matrix
<img width="1096" height="963" alt="confusion_matrix" src="https://github.com/user-attachments/assets/38e53034-1d69-4829-9568-a695dbd39509" />
