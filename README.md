# This is a kaggle project named [Bengali Handwritten Digit Recognition] (https://www.kaggle.com/c/numta)
**Pipeline :**<br>
All train images (augmented and raw images) are appended in X_train after processing and all the labels for the train
(augmented and raw images) images are stored in the y_train.<br ><br>

**Processing:**<br >
All the images are resized first to 28x28 pixel , then the images are blurred and then de-blurred to remove background
noises then again the images are filtered to remove noise further and lastly the images are converted in binary image.<br>
	
Then I augment the images to increase the train set , the augmentation that is used is random rotation , shearing, ZCA whitening,
blur, width shit, height shift and width-height shift(together) . These augmentation is implemented in every image of the train 
dataset , so datasets are multiplied by 7 times.<br><br>

**Model:**<br>
I used a CNN model in which there are 10 CNN layer and a max pooling layer after every two layers followed by 3 fully connected layers
and the output layer . <br><br>

### ALL THE IMAGES ARE IN THIS DIRECTORY EXACTLY LIKE IN THE "numtaDB" , THE DIFFERENCE IS THAT THE ZIPPED FILES ARE UNZIPPED
IN SUB-FOLDERS ON THE SAME DIRECTORY MENTIONED BELOW. All the images are in the following directory follow the exact dataset structure of
the dataset of "[numtaDB]"(https://www.kaggle.com/BengaliAI/numta)<br>
* G:/Numta_Workshop/Numta_Workshop/

### The code is written in "python 3.5" which uses the external packages as follows:
*Keras
*Tensorflow
*Numpy
*Matplotlib
*Opencv
*Pandas