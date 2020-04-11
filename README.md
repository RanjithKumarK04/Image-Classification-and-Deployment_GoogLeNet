# Image-Classification-and-Deployment_GoogLeNet
This repository comprises of training GoogLeNet from scratch on Cifar10 and then using Flask for Model serving

In this Repository, we have GoogLeNet(Inception V1) Model.

We have used this model on Cifar10 dataset to train the model. for training, code is in Training_Notebook.ipynb file.

Inference.ipynb contain Inference code, where we have stored 10 images randomly from Cifar10 testing dataset and predicted using GoogLeNet model.

training_data.py contain Cifar10 dataset (with some transformations on training data).

build_model.py contain GoogLeNet model which is used during Training and Inference.

train.py contain training details like optimizer, epochs, file logger, training and validation loss calculation.

app.py is useful in predicting the class of Image.

run below commands in command prompt

1. cd data
2. python generate_valid_data.py
3. python flask_api/app.py
