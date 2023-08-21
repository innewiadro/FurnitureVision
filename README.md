# FurnitureVision
The aim of this project is to create a simple convolutional network to recognize and classify type of furniture.

## Table of Contents
* [General Infomation](#general-information)
* [Technologies](#technologies)
* [Features](#features)
* [Setup and Usage](#setup-and-usage)
* [Models](#models)
* [Project Status](#project-status)
* [Sources](#sources)
* [Room for Improvement](#room-for-improvement)
* [Contact](#contact)


## General Information
The idea behind this project is to create a model that can predict which specific type of furniture is there based on images.

The use of CNNs is appropriate for this project because these networks are very effective at recognising objects from images. By training the CNN model on a training set, it will be able to learn to extract features from different types of furniture and recognise them accurately in new images.

## Technologies
Project is created with:
- python==3.10
- numpy==1.23.5
- pandas==1.5.3
- scikit-learn==1.2.2
- scipy==1.10.1
- tensorflow==2.12.0


## Features
- Downloads furniture images from the BlackRedWhite website.
- Utilizes advanced machine learning techniques, particularly CNNs.
- Explores various model parameters for optimal performance.

## Setup and Usage

This chapter describes how to use your project in Google Colab.

1. **Step 1:** Clone this notebook into your Google Colab account.
2. **Step 2:** Open the notebook in Google Colab.
3. **Step 3:** Follow the steps in the notebook to see the results of your project.
4. **Step 4:** It is possible to load models and the training history.
To do this you will need to create folders on your Google Drive and copy the published models and training histories.
Folder paths to create are e.g. :

```
'drive/MyDrive/project_computer_vision/model'
'drive/MyDrive/project_computer_vision/history'
```

These can be created using the command:
```
os.makedirs('drive/MyDrive/project_computer_vision/model/', exist_ok=True)
os.makedirs('drive/MyDrive/project_computer_vision/history', exist_ok=True)
```
Then load the model and history using the load_all_models and load_history functions.

**The files model_2.keras, model_8.keras and model_9.keras as well as history_2.npy, history_8.npy and history_9.npy are not placed in the repository as they take up too much space.**

## Models
Models created in this project:
1. 'Basic model': A simple baseline model using fundamental parameters.
2. 'Increased number of neurons': Model with an increased number of neurons in layers.
3. 'Reduced number of neurons': Model with a decreased number of neurons in layers.
4. 'Kernel size (4, 4)': Model with larger convolutional kernel size (4x4).
5. 'Dropout (0.5)' (25 epochs): Model with dropout layers having a rate of 0.5 trained for 25 epochs.
6. 'Dropout (0.5) (50 epochs ': Model with dropout layers having a rate of 0.5 trained for 50 epochs.
7. 'Regularisation (0.01)': Model with regularization at a rate of 0.01.
8. 'Transfer Learning (epochs = 10)': Model utilizing transfer learning, trained for 10 epochs.
9. 'Transfer Learning (epochs = 25)': Model utilizing transfer learning, trained for 25 epochs.

## Project Status
The project is currently in progress. Future plans include the addition of new features to enhance its capabilities. Stay tuned for updates and exciting enhancements!

## Sources
The data to create the programme are taken from www.brw.pl.

## Room for Improvement

To do:
- Increasing the amount of data available 
- Use augmentation techniques such as shifts, rotations or reflections to increase the variety of data and improve the model's ability to generalise.
- Choosing the right hyperparameters can have a significant impact on the performance of the model. Different parameter values can be experimented with, such as number of convolutional layers, number of filters, filter sizes, dropout rate, learning rate.
- Instead of using a single division of the set into training and validation sets, cross-validation can be used, which allows a more accurate estimation of model performance. This can help to avoid accidental splits that may affect the results.
- Use an image pre-processing technique, such as batch normalisation, to match the input images to the expectations of the model.


## Contact
Created by [micwoszk@wp.pl] - feel free to contact me!

