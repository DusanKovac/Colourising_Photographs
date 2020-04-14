# Colourising Images using CNN's

In this project, three different implementations of CNN's were tested. One 
using 6 layers, one using VGG19's layers, and a final one implementing Zhang et al. Colourising Images CNN

![Model 3's Results](https://github.com/DusanKovac/Colourising_Photographs/blob/master/Model%203%20results.jpg)

Important: Please set your current working directory at the start of each notebook, or it will not work!

## Requirements:
To run this are Jupyter, NumPy, SciPy, Keras/Tensorflow, and numerous other smaller packages

Each folder contains its own model, using the data in Data/original for Models 1 and 2 or Data/Lab_origin for Model 3, the Jupyter notebook will run and train a model, every 20 epochs the output will be sent to outputs/ModelX/epoch(number).

Once all models are trained, you may extract for models 1 and 2 the weights from the file contained in the epoch file, for model 3 it will output the model to the Model3 file. 

Running the Test files will, currently, colourise photos from /example_input/p_(512/256) and if you want you may add more photographs. The current ones are downloaded from British Columbian Web archives.

# NOTE:
If you ever want to retrain the files, you must delete all epoch files in outputs/ModelX/epoch* . Or the OS package will throw out an error.

## /Data
Contains 512x512 images in /Lab_origin and 256x256 in original files, the other files will be filled by NumPy arrays produced in Data Preprocessing

## /Data Pre_Process
Contains a notebook which will convert all image data into NumPy arrays and save them in the corrosponding and generate text files containing the names of arrays to be used for training or validation.
 
## /Model1
Contains Model1 and Model1_test Jupyter notebooks.

## /Model2
Contains Model2 and Model2_test Jupyter notebooks.

## /Model3
Contains Model3 and Model3_test Jupyter notebooks.

## /outputs

Takes outputs of model training.
For models 1 and 2, the output is outputed into epoch folders, containing the validation and training images that were processed and also the weights stored in a .h5 file.

For model 3 it only savees the weights in its model3 folder. You need to run model3_test to output to model3's output folder.

## /example_inputs

Currently contains folders to put 256x256 or 512x512 images.

## /Test_output

It will take the modelX_test outputs which were originally images in /example_inputs/, and then for each model it has its own file.