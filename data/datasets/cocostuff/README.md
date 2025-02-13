# COCO-Stuff

This is an instruction for setting up COCO-Stuff dataset.
COCO-Stuff 164k is the latest version and recommended.

![](../../../docs/datasets/cocostuff.png)

## COCO-Stuff 164k

### Setup

1. Run the script below to download the dataset (20GB+).

```sh
$ bash ./scripts/setup_cocostuff164k.sh [PATH TO DOWNLOAD]
```

2. Set the path to the dataset in ```configs/cocostuff164k.yaml```.

```yaml
DATASET: cocostuff164k
    ROOT: # <- Write here
...
```

### Dataset structure

```
ProtoSegFolder
├── proto-segmentation
│   ├── deeplab_pytorch
│   └── all other elements of the cloned repository
└── datasets
    ├── cityscapes
    │   ├── gtfine
    │   └── leftImg8Bit
    └── task07_pancreas
        ├── ImagesTs
        ├── ImagesTr
        ├── labelsTr
        └── etc
```

## COCO-Stuff 10k

### Setup

1. Run the script below to download the dataset (2GB).

```sh
$ bash ./scripts/setup_cocostuff10k.sh [PATH TO DOWNLOAD]
```

2. Set the path to the dataset in ```configs/cocostuff10k.yaml```.

```yaml
DATASET: cocostuff10k
    ROOT: # <- Write here
...
```

### Dataset structure

```
├── images
│   ├── COCO_train2014_000000000077.jpg
│   └── ...
├── annotations
│   ├── COCO_train2014_000000000077.mat
│   └── ...
└── imageLists
    ├── all.txt
    ├── test.txt
    └── train.txt
```
