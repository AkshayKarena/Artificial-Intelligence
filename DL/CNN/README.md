**Fasion Classification Using CNN**
In this project, build a CNN architecture to classify Fasion Images.

Project Overview
  - Dataset: Fashion-MNIST (Kaggle)

  - Framework: TensorFlow / Keras

  - Model: CNN (Convolutional Neural Network)

  - Platform: Google Colab

**Data-Set**
Data-Set is download from Kaggel, in this data-set has 10 classes and all images are in flatten form.
Data-set Link:-https://www.kaggle.com/competitions/iitm-dl18-pa1/data?select=train.csv

**Model Architecture**
**Conv2D:-** filters 32 (for extract feactures)
**MaxPooling2D:-** To reduce dimention
**Conv2D:-** filters 64
**MaxPooling2D:-**
**Conv2D:-** filters 128
**Flatten:-** to convert 2D data into 1D
**Fully connected Neural Network**
**First Hidden Layer** 100 neurons with activation function "relu"
**Second Hidden Layer** 100 neurons with actiovation function "relu"
**Third Hidden Layer** 100 Neurons with actiovation function "relu"
**Output Layer** 10 neurons with activation function "Softmax"

In this project i tried Adam, Momentum and nesterov Optimizer to compair which optimizer is working best.
**Adan Optimizer**
Training Accuracy:-97.40%
Validation Accuracy:- 91.25%

**Momentum Optimizer**
Training Accuracy:- 92.24%
Validation Accuracy:-90.35%

**Nesterov Optimizer**
Training Accuaracy:-92.38%
Validation Accuracy:-89.52%
