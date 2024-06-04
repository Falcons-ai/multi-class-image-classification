<div id="top"></div>
<div align="center">

[![Generic badge](https://img.shields.io/badge/FALCONS.AI-Computer_Vision-red.svg)](https://shields.io/)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)

</div>



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/mstatt/image_dataset_prep">
    <img src="assets/fai_gradient_logo.png" alt="Logo" >
  </a>
</div>



# Multi-Class Computer Vision image classification by Falcons.ai

Welcome to the Multi-Class Computer Vision image classification project by Falcons.ai. This repository contains Jupyter notebooks for preparing an image dataset and training/testing a Multi-Class Computer Vision image classification model using TensorFlow and/or PyTorch.

## Overview
The goal of this is to prepare an image dataset and train a image classification model. The system will be trained on an image dataset of your choosing and will be capable of classifying a range of images from the classes you specify.

We use TensorFlow or PyTorch, powerful open-source libraries for machine learning, to build and train the model.

- ## ** This entire code structure was designed to facilitate from 2 -20 or more classes and be as dynamic as possible. **

## Directory Structure
```
Ensure that your data directory contains subfolders named according to each class of images. For example:

data_directory/
├── class1/
    ├── image1.jpg
    ├── image2.jpg
    ├── etc
├── class2/
    ├── image1.jpg
    ├── image2.jpg
    ├── etc
└── class3/
    ├── image1.jpg
    ├── image2.jpg
    ├── etc
etc
```
** Folder names should be lowercase without spaces **

## Installation

```
pip install -r requirements.txt
```

1. Run the image_utilities notebook

2. Run the tensorflow_model_trainer.ipynb

  or Run the pytorch_model_trainer.ipynb



## Usage
### 1. Data Preparation
First, prepare the dataset by running the `image_utilities.ipynb` notebook. This notebook will:
- Load the raw image dataset.
- Perform preprocessing tasks such as cleaning, balancing, resizing, normalization, and augmentation.
- The notebook will also split the data into training and validation sets for you.
- The processed data will be saved in the in the `data_directory/` directory.


To run the notebook:
```bash
jupyter notebook image_utilities.ipynb
```

### 2. Model Training and Testing
After preparing the dataset, train and test the model by running the `tensorflow_model_trainer.ipynb` or `pytorch_model_trainer.ipynb` notebook. This notebook will:
- Define the neural network architecture using TensorFlow.
- Train the model on the processed dataset.
- Evaluate the model's performance on a test set.
- Save the trained model to the `model/` directory.
- Test the model using images 0-5

To run the notebook:
```bash
jupyter notebook tensorflow_model_trainer.ipynb

or

jupyter notebook pytorch_model_trainer.ipynb
```

## Results
- The data distribution will be generated and saved as images.
- The training metrics and confusion matrix will be generated as images.
- The trained model, will be saved in the `model/`  directory.

## Contributing
Contributions are welcome! If you would like to contribute to this project, please:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

<!-- LICENSE -->
## License

![](https://img.shields.io/badge/License-MIT-blue)


---
