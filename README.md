# Colourising Images using CNN's

## In this project, three different implementations of CNN's were tested. One 
## using 6 layers, one using VGG19's layers, and a final one implementing Zhang et al. Colourising Images CNN


## Requirements to run this are Jupyter, NumPy, SciPy, Keras/Tensorflow, and numerous other smaller packages

# Important: Please set your current working directory at the start of each notebook, or it will not work!

## Each folder contains its own model, using the data in Data/original for Models 1 and 2 or Data/Lab_origin for Model 3, the Jupyter notebook
## will run and train a model, every 20 epochs the output will be sent to outputs/ModelX/epoch(number).

## Once all models are trained, you may extract for models 1 and 2 the weights from the file contained in the epoch file, for model 3 it will output the model to
## the Model3 file. 

## Running the Test files will, currently, colourise photos from /example_input/p_(512/256) and if you want you may add more photographs. The current ones are downloaded from British Columbian
## Web archives.

# NOTE:
## If you ever want to retrain the files, you must delete all epoch files in outputs/ModelX/epoch* . Or the OS package will through out an error.