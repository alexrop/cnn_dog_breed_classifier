# Table of Contents

1. [Overview](#overview)
2. [Installation](#installation)
3. [Project Motivation](#motivation)
4. [File Descriptions](#files)
5. [Results](#results)
6. [Licensing, Authors, and Acknowledgements](#licensing)


---

# Overview <a name="overview"></a>

In this project we apply real Deep Learning conncepts to build a pipeline to process real-world, user-supplied images. Given an image of a dog, the Convolutional Neural Networks (CNN) model will be able identify an estimate of the canine’s breed. If supplied an image of a human, the code will identify the resembling dog breed.


# Installation <a name="installation"></a>

This project uses Python 3.6.3. The following libraries are necessary for running the files: 

  - opencv-python==3.2.0.6
  - h5py==2.6.0
  - matplotlib==2.0.0
  - seaborn==0.8.1
  - numpy==1.12.0
  - scipy==0.18.1
  - tqdm==4.11.2
  - keras==2.0.2
  - scikit-learn==0.18.1
  - pillow==4.0.0
  - ipykernel==4.6.1
  - tensorflow==1.0.0

### Instructions:

1. Clone this github repository.
`https://github.com/alexrop/cnn_dog_breed_classifier.git`

2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip). Unzip the folder and prepare image label pairs for training the model.

3. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip). Unzip the folder and prepare images for the face detector model.

> I highly recommend working on virtual environments as [conda](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#activating-an-environment) or [venv](https://docs.python.org/3.6/library/venv.html) 


# Project Motivation <a name="motivation"></a>

Nowadays we are surrounded by new technologies, where we only need to look at self-driving cars to realize that the future is approaching fast. One of the main reasons I started this project was to understand al least the basics concepts of Deep Learnig ad Neural Networks, and how it is so useful in real life. 

On the other hand, another main motivation was to apply all the knowledge from the Udacity DSNP. It was challenging at first, but after trying and making mistakes (and fixing them), the final goal was achived. 


# File Descriptions <a name="files"></a>

The following is the distribution of the files inside this repo.

```
cnn_dog_breed_classifier
    |-- bottleneck_features
          |-- Readme.txt --> Instruction how to install the features (850 MB and 1.7 GB)
    |-- haarcascades
          |-- haarcascade_frontalface_alt.xml  --> extract pre-trained face detector
    |-- images
          |-- Multiple images  --> Images for test and notebook
    |-- requirements
          |-- Linux | Mac | Windows  --> Programs needed to execute the notebook
    |-- saved_models
          |-- InceptionV3_model.weights.best.hdf5   --> Models output from the notebook that can be pointed
          |-- weights.best.from_scratch.hdf5 
          |-- weights.best.VGG16.hdf5 
    |-- dog_app.html  --> HTML of the jupyter notebook
    |-- dog_app.ipynb --> Jupyter notebook
    |-- extract_bottleneck_features.py

```
The structure of the notebook is as follows:

    - Intro
    - Step 0: Import Datasets
    - Step 1: Detect Humans
    - Step 2: Detect Dog
    - Step 3: Create a CNN to Classify Dog Breeds (from Scratch)
    - Step 4: Create a CNN to Classify Dog Breeds (using Transfer Learning)
    - Step 5: Write Your Algorithm
    - Step 6: Test Your Algorithm

# Results <a name="results"></a>

The most important result is the web app that was created. In the "plot" folder you can see the interface and how it works. You can also see the notebooks to get more details.



# Licensing, Authors, Acknowledgements <a name="licensing"></a>

All data and guidelines here were provided by [Udacity](https://www.udacity.com/course/data-scientist-nanodegree--nd025)
Author: Alexander Ulloa Opazo
