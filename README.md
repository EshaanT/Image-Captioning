# Image-Captioning
The goal of this project is to make an automated image descriptor, using deep learning-based  models.
# Dataset
I made use of the Flickr8K dataset. This dataset consists of 8,000 images that are each paired with five cations, which describe the image. The images are general and tend not to contain any well-known people or locations. The images are also divided into rain set (6000 images), validation set(1000 images), and test set (1000 images).  

You can download the data from here: https://github.com/jbrownlee/Datasets/releases
# Model
In the project, we have made use of **InceptionV3** to extract the features from the image and then injected these features into an RNN model in three different ways:-

* *Init-inject*:- In which we initialize the hidden state of the RNN unit using the image vectors.
* *Par-inject*:-  Here we combined the word vectors with the image vectors before feeding them into the RNN model.
* *Merge*:- Here the image vectors are not fed to the RNN models. Instead, the image is introduced into the model after the description has been encoded by the RNN model

