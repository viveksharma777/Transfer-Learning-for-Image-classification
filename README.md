# Transfer-Learning-for-Image-classification
This project leverages transfer learning with the VGG16 model to classify images of cats and dogs from a dataset sourced from Kaggle. It demonstrates data preprocessing, transfer learning techniques, and performance improvement through model fine-tuning.

### Project Objectives
* Utilize VGG16 as a pre-trained model for classifying cat and dog images.
* Apply data preprocessing and augmentation techniques.
* Fine-tune specific layers to improve model generalization.
### Key Features
1. Data Preparation: Dataset split into training, validation, and test sets, with normalization and preprocessing applied.
2. Transfer Learning Setup: Leveraged VGG16 with frozen layers for initial training, then fine-tuned select layers to refine model performance.
3. Regularization:
   * Dropout Layers: Added dropout layers after fully connected layers to mitigate overfitting.
   * Data Augmentation: Used horizontal flips and rescaling to improve training data diversity.
4. Training and Evaluation: Trained the model using binary cross-entropy loss and fine-tuned with a smaller learning rate.

### Usage
1. Clone this repository.
2. Set up the Kaggle API for downloading the dataset, and follow the instructions to place it in the correct directory.
3. Preprocess the dataset and prepare the model architecture as outlined in train_model.py.
4. Train the model using the fit function, then evaluate its performance on the test set.
