# Image Classifier using VGGNET
This repository contains the final project for  [AI Programming with Python](https://www.udacity.com/course/ai-programming-python-nanodegree--nd089) offered by [Udacity](https://www.udacity.com/).The project was built using Pytorch ML library, The Classifier architecture was based on VGGNET and was trained on 102 category flower data provided by vgg group.

The project dealt with building an image classifier almost from scratch. 
* reading and transforming the data
* choosing a suitable (pretrained) network architecture
* defining a suitable classifier for the chosen architecture
* training the neural network
* evaluating the neural network
* saving and loading checkpoints of the neural network
* illustrating the predictions visually with the corresponding probabilities

The first goal of the project was to implement the above described functionality in a Jupyter Notebook. 
The second goal was to build a command line application allowing the user to:
* choose different network architectures (`vgg13`, `vgg16`, `alexnet`)
* customize the hyperparameters (epochs, learning_rate, hidden units)
* use a GPU for training (if available)
* save and load the model
* use the model to make predictions

### Training
1. Checkout this repository and navigate into `ImageClassifierApp`
2. Run `python train.py <data_directory>` (the script is written in such a way that the user is informed about all the steps taken (building the network, training, ...))
3. To see all the possible customizations, run `python train.py --h`

### Predicting
1. Checkout this repository and navigate into `ImageClassifierApp`
2. Run `python predict.py <path_to_image> <checkpoint>` (note that a valid checkpoint needs to be given)
3. To see all the possible customizations, run `python predict.py --h`