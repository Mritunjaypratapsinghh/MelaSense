# MelaSense
MelaSense is a repository focused on melanoma classification using a custom Convolutional Neural Network (CNN) implemented with TensorFlow. It includes code for building a multi-class classification model to identify various types of skin cancer, particularly melanoma, using skin lesion images.
## Abstract

Melanoma is one of the deadliest type of skin cancer that exists. There are so many factors which leads to Melanoma, the primary ones include exposure to UV rays, poor immune system, rare genetic conditions, a history of affected family member and others. Melanoma develops in our skin cells called melanocytes. It starts when the healthy cells begin to grow out of control, creating a cancerous tumor. If this is not diagnosed in the early stages the mortality rate reduces to less than 20% where as in early detection the mortality rate is 95%. Melanoma can be cured if diagnosed early, else they spread to other body parts and leads to death.


## Problem Statement
 In the skin biopsy, the dermatologist takes some part of the skin lesion and examines it under the microscope. The current process takes almost a week or more, starting from getting a dermatologist appointment to getting a biopsy report.
 The aims to shorten the current gap to just a couple of days by providing the predictive model.
 The approach uses Convolutional Neural Network (CNN) to classify nine types of skin cancer from outlier lesions images. This reduction of a gap has the opportunity to impact millions of people positively.

## Motivation
The overarching goal is to support the efforts to reduce the death caused by skin cancer. The primary motivation that drives the project is to use the advanced image classification technology for the well-being of the people. Computer vision has made good progress in machine learning and deep learning that are scalable across domains.

## Dataset
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images.

The data set contains the following diseases:

![datasetdf](https://github.com/Mritunjaypratapsinghh/MelaSense/blob/main/Readme_images/Datasetdf.png)

![datasetplot](https://github.com/Mritunjaypratapsinghh/MelaSense/blob/main/Readme_images/DatasetPlot.png)

To overcome the issue of class imbalance, used a python package  Augmentor (https://augmentor.readthedocs.io/en/master/) to add more samples across all classes so that none of the classes have very few samples.

### Sample image from Dataset

![sample image](https://github.com/Mritunjaypratapsinghh/MelaSense/blob/main/Readme_images/Samleimagefromdataset.png)

## CNN Architecture Design
To classify skin cancer using skin lesions images. To achieve higher accuracy and results on the classification task, I have built custom CNN model.

- Rescalling Layer - To rescale an input in the [0, 255] range to be in the [0, 1] range.
- Convolutional Layer - Convolutional layers apply a convolution operation to the input, passing the result to the next layer. A convolution converts all the pixels in its receptive field into a single value. For example, if you would apply a convolution to an image, you will be decreasing the image size as well as bringing all the information in the field together into a single pixel. 
- Pooling Layer - Pooling layers are used to reduce the dimensions of the feature maps. Thus, it reduces the number of parameters to learn and the amount of computation performed in the network. The pooling layer summarises the features present in a region of the feature map generated by a convolution layer.
- Dropout Layer - The Dropout layer randomly sets input units to 0 with a frequency of rate at each step during training time, which helps prevent overfitting.
- Flatten Layer - Flattening is converting the data into a 1-dimensional array for inputting it to the next layer. We flatten the output of the convolutional layers to create a single long feature vector. And it is connected to the final classification model, which is called a fully-connected layer.
- Dense Layer - The dense layer is a neural network layer that is connected deeply, which means each neuron in the dense layer receives input from all neurons of its previous layer.
- Activation Function(ReLU) - The rectified linear activation function or ReLU for short is a piecewise linear function that will output the input directly if it is positive, otherwise, it will output zero.The rectified linear activation function overcomes the vanishing gradient problem, allowing models to learn faster and perform better.
- Activation Function(Softmax) - The softmax function is used as the activation function in the output layer of neural network models that predict a multinomial probability distribution. The main advantage of using Softmax is the output probabilities range. The range will 0 to 1, and the sum of all the probabilities will be equal to one.

### Model Architecture
![Model Arch](https://github.com/Mritunjaypratapsinghh/MelaSense/blob/main/Readme_images/ModelLayer.png)

### Model Evaluation
![ModelEvaluation](https://github.com/Mritunjaypratapsinghh/MelaSense/blob/main/Readme_images/ModelEvaluation.png)


## Homepage
![homepage](https://github.com/Mritunjaypratapsinghh/MelaSense/blob/main/Readme_images/Homepage.png)

## Working
![melanoma](https://github.com/Mritunjaypratapsinghh/MelaSense/blob/main/Readme_images/melanoma.png)
![basalcell](https://github.com/Mritunjaypratapsinghh/MelaSense/blob/main/Readme_images/basalcell.png)

## Installation

To use MelaSense locally, follow these steps:

1. Clone the repository: git clone https://github.com/Mritunjaypratapsinghh/MelaSense.git

2. Install the required dependencies:

3. Run the application:

4. Access MelaSense in your web browser at `http://localhost:5000`.

## Contributing

Contributions to MelaSense are welcome! If you'd like to contribute, please follow these guidelines:

1. Fork the repository and create your branch:

2. Commit your changes and push to your branch:

3. Open a pull request, describing your changes and the motivation behind them.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute it according to the terms of the license.

## Contact

If you have any questions, suggestions, or feedback, please reach out to us. We would love to hear from you!


