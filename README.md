# dli_emotions

NVIDIA IoT [Deep Learning Institute](https://www.nvidia.com/en-us/deep-learning-ai/education/) thumbs image classifier at the edge (IoT) project for Jetson Nano. 

This project is meant to be run at the edge on an NVIDIA Jetson Nano (or similar ARM IoT architecture computer).  

## Requirements
* Jetpack SDK or [DLI Jetson Nano image](https://developer.download.nvidia.com/training/nano/ainano_v1-1-1_20GB_200203B.zip) (preferably the latter for headless mode compatibility)
* [Jetcam](https://github.com/NVIDIA-AI-IOT/jetcam)
* Jupyter Notebooks (AKA IPython)
* Pytorch


## Repository structure ##

### [data](data) 
Contains 200 images times 4 classes (total images = 800) taken and used for training. The images were encrypted for privacy purposes.

### [models](models) 
Contains different model iterations and are named after the total training images and epochs. The best performing model is the *200dpx4_35ep.pth* model which was trained with 200 images per class and for a total of 35 epochs.

### [notebooks](notebooks)
Contains the Jupyter notebook used to interactively train and evaluate a thumbs position (up or down) model using deep learning and PyTorch.

### [src](src)
Standard src scripts and utilities plus a folder structure generator script.

## Usage
Use the interactive notebook from the notebooks folder and train your own model or load one already made from the models folder and evaluate how effective it is using your camera.

## License
[MIT License](https://github.com/socd06/dli_thumbs/blob/master/LICENSE)
