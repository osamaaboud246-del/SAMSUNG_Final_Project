# SAMSUNG_Final_Projec

## 1st stage (Nawal, osama ->preperation +preprocessing) :

### overview

i worked on preparing a dataset of arabic sign language letters. here is a step-by-step explanation of what i did from the beginning.

#### 1. importing the libraries

first, i imported all the python libraries i needed for my work. i added tools to read files from my computer, handle data tables, edit images, draw charts, and prepare the data for a deep learning model. i also printed a simple word at the end to make sure all the libraries loaded without any errors.

#### 2. handling broken images

i changed a setting in the image library to allow loading incomplete image files. did this to stop the code from crashing if it finds a broken picture inside the folders.

#### 3. loading and preparing the images

after that, i set the path to the dataset folder on my computer (localy) and created two empty lists to hold the images and their labels. i made a loop to go through every letter folder and open each image one by one. 

for each picture, i resized it to 224 by 224 pixels so all images have the exact same size. then, i turned the image into a number array and divided the values by 255.0 to make all the numbers stay between 0 and 1. i saved each processed image and its folder name into my lists next i show that.

#### 4. encoding the labels

once all the images were in my list, i used a label encoder to turn the text names of the arabic letters into whole numbers. then, i converted those numbers into categorical vectors so the machine learning model can use them for training later.

#### 5. checking the processed data

Finally, i wrote a script to print out a summary of my work. i checked the total number of loaded images and labels, which was 7856 across 31 different classes. i also printed the shape of a single image, the minimum and maximum pixel values, and the new format of the labels to make sure the preparation step worked properly.
