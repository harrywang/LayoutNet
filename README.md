# About 

The code is revised based on the code and data found at https://xtqiao.com/projects/content_aware_layout/

## Data
Download the three zip files from (link) and extract them into three folders. Your repo should have the following structure:
```
.
├── LICENSE.txt
├── README.md
├── config.py
├── dataset
├── model.py
├── sample
├── test.py
├── train.py
├── trainer_step.py
└── validation
```

## Setup

TODO: add the following to requirements.txt and use virtual environment

* python 2.7
* cuda 9.0
* pillow
* scipy
* tensorflow 1.5.0
* tensorslim


## Training
* ``python train.py``
* Results are generated in the folder ``./example/*.png``
* Models are saved in the folder ``./log/***``

## Testing
* Generate one random noise vector (60*128).
* Change the testing folder in ``inputs()`` from ``./sample/`` to ``./validation/``
* Select the model name in ``testing()``
* ``python test.py``
