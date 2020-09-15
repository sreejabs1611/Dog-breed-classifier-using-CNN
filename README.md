DOG BREED CLASSIFIER USING CNN

This project is to build a CNN (Convolutional Neural Network) to classify different dog breeds. If the image of a dog is found, this algorithm would find the estimate of the breed. We have built a pipeline to process real world images.

Dogs are one of the most common domestic animals. The breed of dogs carries a lot of information, a lot more than just their appearance. 
Dogs of different breeds may have different temperament, different space and climate requirement, different effort and time it takes the owner to train them, different price and feeding cost, and so on. 
Due to a large number of dogs, there are several issues such as population control, decrease outbreak such as Rabies, vaccination control, and legal ownership. Each dog breed has specific characteristics and health conditions. 
In order to provide appropriate treatments and training, it is essential to identify individuals and their breeds. 

Project Process
Import the labelled dataset of the dog breed. 
Process the images to resize them and store them in array of desired format. 
Break the dataset into training & testing dataset. 
Build and train a convolutional neural network on the image dataset of the dog breeds.
Adjust and tune the model until a certain accuracy is achieved.
Once the model is trained, it can be used to predict the class (breed) of any input dog image. 
Experiment the model by increasing number of classes and observe accuracy. 
Results and conclusion

ALGORITHM
Format Custom Image Data to Input to Keras Model
We loop through the images of the dogs for each breed category. 
Since images are kept in their respective breed folder. Hence the each of the images are labelled. 
We load all the images for the category from its folder. 
Resizing Images 
Each of the image is resized to 100x100. This is done to keep dimensions of all the images uniform.  
Prepare dataset 
Each of the categories contain around 150 images. 
Randomly choose 15% of the data from each  category to be part of testing data, and the rest 85% to be training data. Since we have limited data (only 150 images per category) so we will be using the testing data as the validation data as well.
Simple CNN 
Build a model which takes input as the image and trains the model. 
The model is composed of several convolutional layers and the max pooling layer. 
In the end of the layers a dropout is added to prevent the model from being overtrained. 
The last layer is backed by dense layers and number of units in the dense layer is equal to the number of classes.






