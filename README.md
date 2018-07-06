# Training-Mask-RCNN
How to train [Mask RCNN](https://github.com/matterport/Mask_RCNN) on your own dataset.

## Requirements
- Ubuntu 16.04
- Python 3.5
- Tensorflow-gpu 1.8
- Keras 2.1.6

## Getting Started
Creating virtualenv
```bash
$ cd Training-Mask-RCNN
$ virtualenv env --python=python3.5
$ source env/bin/activate
```

Install Dependencies
```bash
$ pip install -r requirements.txt
```

Training on Your Own Dataset
```bash
# Train a new model starting from pre-trained COCO weights
$ python trainer.py train \
    --dataset=/path/to/dataset \
    --weights=coco
```
