# Reverse-Visual-Search
Reverse Visual Search System on MS COCO mini dataset.

[Google drive with data set and notebooks](https://drive.google.com/drive/folders/1o72ar3K5DLBf8Sc7DPSybvJyJKFr9ahC?usp=sharing)

# Set up
This set up works in a linux development environment, and
assumes Tensorflow 2.5 or better has already been installed

## Clone this repository
```
git clone https://github.com/J-Mojica/Reverse-Visual-Search.git
cd Reverse-Visual-Search
```

## Download the [MSCOCO mini dataset](https://github.com/giddyyupp/coco-minitrain)

[Download dataset](https://drive.google.com/file/d/1t_l9uyBPfxSEzcajTk4a1TaQXzeRm9hw/view?usp=sharing)

## Install the Tensorflow Object Detection API

Clone the Tensorflow Models repository with the following command
 ```
git clone --depth 1 https://github.com/tensorflow/models
 ```
##Install the Object Detection API
```
sudo apt install -y protobuf-compiler
cd models/research/
protoc object_detection/protos/*.proto --python_out=.
cp object_detection/packages/tf2/setup.py .
python -m pip install .
```

# Getting the persons bounding boxes in the dataset
[This notebook](https://colab.research.google.com/drive/1-6wAM9ni6d0o9i2tVXoZ2_aoYh9jmDnC?usp=sharing) goes through the process of extracting the 
bounding boxes of only the persons in the data set and outputs
them to a json file.

[Training images person bounding boxes](https://drive.google.com/file/d/1_etICCAyFjs4w3y6FZ6m0hDAHRgSzsQE/view?usp=sharing)
