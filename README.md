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

> We highly recommend to you can instalL all of the programs from above in a virtual environment like conda or venv 


# Project Motivation <a name="motivation"></a>

Nowadays we are surrounded by new technologies, where we only need to look at self-driving cars to realize that the future is approaching fast. One of the main reasons I started this project was to understand al least the basics concepts of Deep Learnig ad Neural Networks, and how it is so useful in real life. 

On the other hand, another main motivation was to apply all the knowledge from the Udacity DSNP. It was challenging at first, but after trying and making mistakes (and fixing them), the final goal was achived. 


# File Descriptions <a name="files"></a>

The following is the distribution of the most important files

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
Inside the notebook the structure is as follows:

The project is divided into 7 steps:

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

Getting started: 

1) Clone this repository and unzip the model 
```
git clone https://github.com/alexrop/disaster_response_figure_eight.git
```
then go to the models folder and unzip the classifier.pkl which is contain in a rar format (100 mb approx)

2) Run the program

```
python run.py
```

3) Web App interface

On terminal type: 
```
env|grep WORK
```

Then go to the following address by completing with your own *SPACEDOMAIN* and *SPACEID*. For example, in my case was *https://view6914b2f4-3001.udacity-student-workspaces.com/*

```
https://SPACEID-3001.SPACEDOMAIN
```

![image](https://user-images.githubusercontent.com/49656060/127645094-0378c288-2c4f-45c6-b7c6-f97c98b4030e.png)

![image](https://user-images.githubusercontent.com/49656060/127645147-937699e0-846f-4bf3-8254-f2268efeb15d.png)


Now, if you want to re-execute the `process_data.py` and `train_classifier.py` scripts, you must follow this nomenclature:

```
python process_data.py disaster_messages.csv disaster_categories.csv disaster_process_data.db
```

```
python train_classifier.py ../data/disaster_process_data.db classifier.pkl
```
>The last one (train_classifier.py) takes around 2 h aprox to be completed


On the other hand, if you need more details about the ETL and ML Pipeline process, check the *notebook* folder,  where you can find a "step-by-step" explination about how we generate the final database and model.

> Note: This project was made on the *Udacity Project Workspace IDE platform* (Ubuntu based) so it might be some differences if you run it on Windows. Check that the package versions are the same that mine as I showed you above.

![image](https://user-images.githubusercontent.com/49656060/127631805-febda984-8554-4906-9c81-efd6525f2c04.png)


# Licensing, Authors, Acknowledgements <a name="licensing"></a>

All data here belongs to the [Figure Eight](https://appen.com/) company, and it was provided by the [Udacity](https://www.udacity.com/course/data-scientist-nanodegree--nd025) team.
Author: Alexander Ulloa Opazo
