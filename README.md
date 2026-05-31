# Cat vs Dog vs Panda Image Classification using Transfer Learning
### Name: KIRAN M P
### Register No: 212224230123
## Project Overview

This project performs image classification using Transfer Learning in PyTorch to classify images into three categories:

* Cat

* Dog

* Panda

The model uses a pre-trained ResNet18 network from TorchVision and fine-tunes the classifier layers for multi-class image classification.

## Dataset
Dataset used:

Cats Dogs Pandas Images Dataset

Kaggle Dataset:

https://www.kaggle.com/datasets/gpiosenka/cats-dogs-pandas-images

Dataset structure:

data/

│── cat/

│── dog/

└── panda/

Images are resized to 224 × 224 and normalized using ImageNet statistics.

## Features
Transfer Learning using ResNet18

CUDA GPU support

Data augmentation

Training and validation split

Best model checkpoint saving

Confusion matrix visualization

Image prediction function

Reproducible results using random seeds

## CUDA Verification

### Run before training:
```
import torch

print("CUDA available:", torch.cuda.is_available())

device = torch.device(
    "cuda"
    if torch.cuda.is_available()
    else "cpu"
)

print(device)
```
## Output:
### Dataset:
<img width="812" height="748" alt="image" src="https://github.com/user-attachments/assets/062a9c95-0798-4103-9b7f-4221228bcd03" />

### ResNet:
<img width="967" height="737" alt="image" src="https://github.com/user-attachments/assets/b1a6333f-8176-43c5-a1c0-cda9fa4694d6" />

### Epochs:
<img width="455" height="330" alt="image" src="https://github.com/user-attachments/assets/cffa85eb-c628-4458-ae64-f60abc8aafde" />

### Accuracy:
<img width="211" height="32" alt="image" src="https://github.com/user-attachments/assets/9541e3c7-dde3-4bf0-93f7-208bb4ab6965" />

### Confusion Matrix:
<img width="923" height="713" alt="image" src="https://github.com/user-attachments/assets/895ddc33-4a8d-4dbb-b34b-5db8178b8084" />
