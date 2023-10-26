# Sign-Language-AI-Translator-
The project is dedicated to translation of sign language into text to overcome the communication barriers between the world and deaf people.
First: - the TF model
The model depends on many blocks:
The first block (1): the keras library from the tensor flow platform was used and Numpy library as it has functions for working in matrices and keras contain two models and it was import from the functional model the main function for classification and detection which is vgg16 then import train-test split and the flatten layer was chosen as the dense layer as it convert 3d image to neuron then import matplotlib to plot the graphs.
The second block (2): it includes the output classes of the test and the place of the dataset and in the testing the result is ŷ then by comparing the y and ŷ it determines the accuracy. 
The third block (3): loading data from image, label, size, and index then the splitting between training image and testing image.
The fourth block (4): determining the batch number which was 128 and the epoch which is =5 and setting the graph data and calculation of the loss by the loss function loss (ŷ , y ) = - (y log(ŷ)) + (1-y) log (1-ŷ). 
The fifth block (5): setting the model then output the testing accuracy, time, and loss. 
Second: -the TF model was covert to Tflite by the official Tflite converter then the Tflite model was put in the react native as it has camera view that take photo and get it in the model.
