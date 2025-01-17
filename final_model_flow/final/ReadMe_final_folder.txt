The given below descriptions and instructions are for the .pynb files present in the "Final" Folder.


Files Present:

main.ipynb : This file is the connector code that connects and runs the functions and models present in the other .pynb files present in the     folder.

chunks_creation_1.ipynb : This is the .ipynb file that is responsible for creating chunks of the image theat the user gives in the destination folder(also given by the user)

gabor_chunk.ipynb : This is used to calculate the gabor values which act as features for the models and store them in an excel. This code also deletes the chunks after execution.

ML_Image_classification_ensembling_image.ipynb : This is the code file that contains the models required to classify the chunks created and from the classified chunks, find the classification of the image as a whole.

enhance.ipynb : This is the code that takes the original image and its classification as input and give its appropriate enhanced image based on its classification. 

patches_gabor_15816_1 3.csv : This is the dataset that is used for training the classification models.






Instructions to run the project: 

Step 1: Ensure that all the .ipynb files are in the same folder.

Step 2: Open the "main.ipynb" file in jupyter notebook.

Step 3: Run the file.

Step 4: Enter the path of the original image, the destination path where all the reports have to be stored and the path of the "patches_gabor_15816_1 3.csv" dataset. 

Important point: the paths when being entered SHOULD NOT be entered in quotes

Step 5: the outputs will be displayed in the notebook and the necessary files will be created and stored in the destination path and the enhanced image will be stored in the same directory as the original image


