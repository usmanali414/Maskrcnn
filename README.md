## Maskrcnn with tf-gpu 1.15.2 and RTX 3090
This Guide will help you to setup Maskrcnn training code on RTX3090 with TF-gpu=1.15.2

### Steps
1- First you need to setup anaconda and create an environment with python==3.8.0

2- install cudatoolkit=11.1.1 with thic command: conda install cudatoolkit==11.1.1 -c conda forge

3- Then install cudnn compatible with cuda11 conda install cudnn==8.4.1.50 -c conda-forge

4- Install tensorflow compiled by nvidia. You need to add chanells in your pip to download nvidia compiled tensorflow. pip install nvidia-pyindex pip install nvidia-tensorflow[horovod]

5- Now install following libraries with mentioned versions: keras==2.0.8 h5py==2.10.0 scikit-image==0.16.2 imgaug ipython

6- Clone this repo in you project folder with this command: "git clone "https://github.com/SriRamGovardhanam/wastedata-Mask_RCNN-multiple-classes.git"

7- build and install after cloning this repo: %cd ./wastedata-Mask_RCNN-multiple-classes/main/Mask_RCNN !pip install -e .

Note: Please before installing libraries make sure you are installing them with the right environment pip. you can check your pip by running command "which pip". If the output is something like this home//anaconda3/envs/<your_en_name>/bin/pip" then your pip is correct and you may carry on installing the libraries.

### Credits:
https://github.com/SriRamGovardhanam https://github.com/anshkumar
