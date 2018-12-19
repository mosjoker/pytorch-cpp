# PyTorch-cpp

## Introduction

Loading a pytorch model in C++.

## Installation

###  Requirements
- PyTorch 1.0 and torchvision 0.2.1
- OpenCV
- Python 3

### Install
a. Download LibTorch [here](https://pytorch.org) and unzip.

b. Clone the repository.
```shell
git clone https://github.com/mosjoker/pytorch-cpp.git 
```
c. Cmake
```shell
cd pytorch-cpp 
mkdir build && cd build
cmake -DCMAKE_PREFIX_PATH=/path/to/libtorch ..
make
```


### Converting your pytorch model to torch script

This examples shows how to convert a resnet18 model. 
```shell
python tools/convert.py
```

### Test 
```shell
./example-app ../model.pt ../dog.png ../synset_words.txt
```

