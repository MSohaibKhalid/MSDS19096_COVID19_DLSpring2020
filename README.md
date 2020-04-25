# Detecting Coronavirus Infections through Chest X-Ray images
---

## Dataset
- Access dataset from [here](https://drive.google.com/drive/folders/1P11biqCGNk5zWqILLdNkuPtbZpvXb1ay?usp=sharing).

## Description about Models used:
Two Models were used: VGG16 and ResNet18 with modiftication in Fully connected layers.

### Fully Connected layers where modified for VGG16 as:
```
    (0): Linear(in_features=25088, out_features=1060, bias=True)
    (1): ReLU(inplace=True)
    (2): Dropout(p=0.5, inplace=False)
    (3): Linear(in_features=1060, out_features=2, bias=True)
```

### Fully Connected layers where modified for ResNet18 as:
```
    (0): Linear(in_features=512, out_features=1060, bias=True)
    (1): ReLU(inplace=True)
    (2): Dropout(p=0.5, inplace=False)
    (3): Linear(in_features=1060, out_features=2, bias=True)
```
