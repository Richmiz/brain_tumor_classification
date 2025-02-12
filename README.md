# Brain Tumor Classification using Deep Learning

This project demonstrates the implementation of a deep learning model for classifying brain tumor images. 
It uses a Convolutional Neural Network (CNN) trained on a dataset of brain tumor images to predict whether an image contains a tumor or not.

## Project Structure

- **ImageClassificationPipeline.py:** Contains the Python class defining the image classification pipeline, including data loading, model definition, training, and evaluation.
- **Brain_Tumur/Brain Tumor Data Set:** Directory containing the brain tumor dataset. This dataset is expected to have two subdirectories, 'yes' and 'no', for images with and without tumors, respectively.
- **model.h5:** File where the trained model will be saved.

## Requirements

- Python 3.6+
- TensorFlow 2.0+
- Keras
- NumPy
- Matplotlib

## Installation

1. Install the required libraries using pip:

2. Mount your Google Drive to Colab:

## Usage

1. Update the `dataset_path` and `model_save_path` variables in the `ImageClassificationPipeline.py` file to point to your dataset directory and desired model save location.
2. Run the script `ImageClassificationPipeline.py` to execute the pipeline.
3. The script will mount your Google Drive, initialize data generators, define the CNN model, train the model, and plot the training history.
4. The trained model will be saved to the specified `model_save_path`.

## Methodology

The project follows these steps:

1. **Data Loading:** Images are loaded from the dataset using the `ImageDataGenerator` class from Keras. Data augmentation is applied to increase the dataset size and improve model generalization.
2. **Model Definition:** A CNN model is defined using Keras layers such as `Conv2D`, `MaxPooling2D`, `Flatten`, and `Dense`. The model is compiled with the Adam optimizer and BinaryCrossentropy loss function.
3. **Training:** The model is trained on the training data using the `fit` method. Early stopping is used to prevent overfitting.
4. **Evaluation:** The model's performance is evaluated on the validation data using metrics such as accuracy. Training and validation accuracy and loss are plotted for visualization.
5. **Saving:** The trained model is saved to an .h5 file for later use.

## Results

The performance of the model is evaluated based on accuracy and loss metrics. The training and validation curves provide insights into the model's learning process and generalization ability.

## Contributing

Contributions to the project are welcome. You can contribute by:

- Improving the model architecture or training process.
- Adding new features or functionality.
- Fixing bugs or issues.
- Providing feedback or suggestions.
