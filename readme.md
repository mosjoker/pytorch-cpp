# PyTorch-cpp

## Introduction

Loading a pytorch model in C++.

## Installation

###  Requirements
- PyTorch 1.0 and torchvision 0.2.1
- OpenCV

### Install
a. Download LibTorch here and unzip
b. Clone the repository.
```shell
git clone 
```
c. Cmake
```shell
cd pytorch-cpp && mkdir build
cd build
cmake -DCMAKE_PREFIX_PATH=/Users/hankai/code/cpp-pytorch/libtorch ..
make
```

### Test
```shell
./example-app ../model.pt ../dog.png ../synset_words.txt
```


