# Cat vs. Dog Image Classification

This project implements a Convolutional Neural Network (CNN) to classify images of cats and dogs using Keras and TensorFlow. The dataset used is sourced from Kaggle.

## Dataset

**Source**: [Cat & Dog Images for Classification](https://www.kaggle.com/c/dogs-vs-cats)

The dataset contains labeled images of cats and dogs used for binary classification.

## Requirements

Make sure you have the following dependencies installed before running the project:

**pip install -r requirements.txt**

## The model consists of:

    Data Augmentation: Random horizontal and vertical flips, random zoom.
    Convolutional Layers: 4 Conv2D layers with ReLU activation and max pooling.
    Dropout Layers: To prevent overfitting.
    Batch Normalization: For stable training.
    Fully Connected Layers: A dense layer with 512 neurons and ReLU activation.
    Output Layer: A single neuron with sigmoid activation for binary classification.

## Training Process

    Dataset Loading: Images are loaded, resized to 64x64, and normalized.
    Train-Test Split: The dataset is split into training, validation, and test sets.
    Model Training: The model is compiled with binary cross-entropy loss and Adam optimizer.
    Evaluation: The trained model is evaluated on the test set.
    Visualization: Training history is plotted.
    Saving the Model: The model is saved as model.h5 if the user confirms.

## Running the Project

To train and evaluate the model, run:

python main/model.py

During execution, the training progress will be displayed, followed by test evaluation results. The trained model can be saved for future use.

Example Output:

Model Summary
...
Epoch 1/50
...
SCORE: [loss, accuracy]

## Future Improvements

    Implementing more advanced data augmentation techniques.
    Adding more convolutional layers for better accuracy.
    Fine-tuning with pre-trained models (e.g., VGG16, ResNet).

## License

This project is open-source and available for personal and academic use.