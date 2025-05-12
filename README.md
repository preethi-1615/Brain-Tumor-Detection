Brain Tumor Classification using CNN

This project performs image-based brain tumor classification into four categories: glioma, meningioma, pituitary, and no tumor. It uses a Convolutional Neural Network (CNN) built with TensorFlow/Keras and provides a user-friendly interface through Gradio.

 Features

- Classifies brain tumor MRI images into one of four categories.
- CNN model with Conv2D, BatchNormalization, and Dropout layers.
- Built-in data preprocessing and augmentation.
- Interactive Gradio web UI for testing with new images.

Dataset Structure

The dataset should be organized as follows under `Training/`:

Training/
├── glioma/
├── meningioma/
├── notumor/
└── pituitary/

Each folder should contain MRI images of the respective category.

Dependencies

Make sure you have the following Python packages installed:

pip install gradio numpy opencv-python tensorflow scikit-learn

How It Works

1. Preprocess Dataset: Images are resized to 128x128, normalized, and labels are one-hot encoded.
2. Train/Test Split: Dataset split into 80% training and 20% testing.
3. Model Training: CNN is trained for 10 epochs with batch size of 16.
4. Prediction Function: Accepts an image, processes it, and returns the predicted tumor type.
5. Gradio Interface: A web UI allows users to upload MRI images and get predictions.

Usage

You can run the program in a Python environment (e.g., Google Colab) using:

!pip install gradio
Then run the script

Or simply execute the Python script after modifying the `DATASET_PATH` to your local dataset directory.

Output Example

When you run the script, a Gradio interface will appear. You can upload an MRI scan image and get an output label like:

Prediction: glioma

Notes

- The model can be improved with more data, augmentation, and tuning.
- If using Colab, ensure that Google Drive is mounted correctly and dataset path is accessible.



Author

Created by: Bala Preethi M 
Contact: balapreethi1615@gmail.com  
GitHub: https://github.com/preethi-1615
