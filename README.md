# Detecting Coronavirus Infections through Chest X-Ray images

## Dataset
Access dataset from [here](https://drive.google.com/drive/folders/1P11biqCGNk5zWqILLdNkuPtbZpvXb1ay?usp=sharing).

## Description about Models used:
Two Models were used: VGG16 and ResNet18 with modiftication in Fully connected layers.

#### Fully Connected layers modified for VGG16 as:
```
    (0): Linear(in_features=25088, out_features=1060, bias=True)
    (1): ReLU(inplace=True)
    (2): Dropout(p=0.5, inplace=False)
    (3): Linear(in_features=1060, out_features=2, bias=True)
```

#### Fully Connected layers modified for ResNet18 as:
```
    (0): Linear(in_features=512, out_features=1060, bias=True)
    (1): ReLU(inplace=True)
    (2): Dropout(p=0.5, inplace=False)
    (3): Linear(in_features=1060, out_features=2, bias=True)
```

## Get Trained Models
Download trained models using following links
* VGG16 Entire: [Download](https://drive.google.com/file/d/1-2MPtBDxXBEK_a1hkv-lmty0AZhOplR-/view?usp=sharing)
* ResNet18 Entire: [Download](https://drive.google.com/file/d/1-2uOOHnIDZuX8JiffRnt1XLbgMMjIFUZ/view?usp=sharing)
* VGG16 FC Only: [Download](https://drive.google.com/file/d/1hJI86eA9Sb9n0Z4hBBdRd9KsI3dZliNb/view?usp=sharing)
* ResNet18 FC Only : [Download](https://drive.google.com/file/d/1-09GoYnB8zTZMhhr1NnGbYRHza3ooX1t/view?usp=sharing)

## Results
#### Confusion Matrices and F1 Scores
![](Results/Vgg16_Entire.JPG)
```
** Best val acc results **
train ==> Loss: 0.3007 , Acc: 87.65 %
val ==> Loss: 0.2924 , Acc: 88.93 %
Testing Data accuracy: 94 %
```
![](Results/Resnet18_Entire.JPG)
![](Results/Vgg_FC_Only.JPG)
![](Results/Resnet18_FC_Only.JPG)
