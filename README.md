# 3DMOD
Creating 3D Model from 2D Images using Convolution Neural Network 

This repository contains the source codes for the paper, "Creating 3D Model from 2D Images using Convolution Neural Network". Using a set of 2D images taken from multiple viewpoints, the features of the object is extracted using CNN from which 3D overview of the object is determined with the help of machine learning. 

Project Paper
The project page is available at
https://drive.google.com/file/d/1-dRAiLNx0RLuJMAm37ykCeUoCk2faFu5/view?usp=sharing 

Project Report
The project report is available at
https://drive.google.com/file/d/10SVNYYOe3Uhh_klmy-ZYYbxh0_fzQWC4/view?usp=sharing

Overview

Main objective of this project was to create a 3D model from 2D input images using Convolutional neural networks. Using a set of 2D images taken from multiple viewpoint the features of the object is extracted using CNN from which 3D overview of the object is determined with the help of machine lerning. The main reason of using CNN is its ability of Feature Learning.

2D images are taken as input which are the digitally processed to extract the important features. These images are passed through a series of convolutional and pooling layers (encoder) after which those values are passed into the aggration model to take out the important features and finally those features are proceed through another series of deconvolutional and pooling layers (decoder) to get the predicted 3D model of given put images.

The use of 3D model has been increasing exponentially in the fields of manufacturing, education, prosthetics and many more 3D models are proved to provide easy and cost-efficient methed to the industries. Many industries are shifting their focus from traditional methods to 3D modelling.

Though the use of 3D models have been convenient, developing it is still a huge challenge. With this project we aim to make the development of 3D models easier and more effective which can be used primarily in visual imagery and other related fields.


Datasets
For training, we used ShapeNet data set which is a gathering of 3D CAD models that are arranged according to the WorldNet hierarchy. We only used subset of the ShapeNet dataset which contains 50000 models and 13 major categories. We split the dataset into 4:1 ratio for training/testing data.
ShapeNet rendered images:
http://cvgl.stanford.edu/data2/ShapeNetRendering.tgz

Requirements

python 3.5
tensorflow 1.2 +
numpy 1.13.3
scipy 0.19.0
matplotlib 2.0.2
skimage 0.13.0

Installation of requirements

Installing Conda
Following steps have to be followed to install conda and create its virtual environment.
1. Download most recent version of Anaconda from
https://www.anaconda.com/download/
2. Download Anaconda Bash Script in /tmp folder using commands
	$ cd /tmp
	$ curl -O https://repo.anaconda.com/archive/Anaconda3-2019.03-Linux-x86_64.sh
3. Run Anaconda Script using following command
	$ bash Anaconda3-2019.03-Linux-x86_64.sh
4. Activate Installation
	$ source ~/.bashrc
5. Test Installation
	$ conda list
6. Create Anaconda Environment
	$ conda create –n 2Dto3D python=3.5
7. Activate new enxironment using
	$ conda activate 2Dto3D

Installing Python
Following steps have to be followed to install python in Ubuntu. Python 3.5 version is used in this project.
1. Update packages list
	$ sudo apt update
	$sudo apt install software-properties-common
2. Add deadsnakes PPA to sources list
$ sudo add-apt-repository ppa:deadsnakes/ppa
3. Install python using
	$ sudo apt install python==3.5

Installing tensorflow-gpu
Following command can be used to install tensorflow-gpu. Tensorflow version 1.2 + is used in this project.
	$ conda install tensorflow-gpu

Installing numpy
Following command is used for installing numpy. Numpy version 1.13.3 is used in this project.
$ conda install numpy==1.13.3

Installing scipy
Following command is used for installing scipy. Scipy version 0.19.0 is used in this project.
	$ conda install scipy==0.19.0

Installing matplotlib
Following command is used for installing matplotlib. Matplotlib version 2.0.2 is used in this project.
$ conda install matplotlib==2.0.2

Installing scikit-image
Following command is used for installing scikit-image. Scikit-image version 0.13.0 is used in this project.
	$ conda install scikit-image==0.13.0







