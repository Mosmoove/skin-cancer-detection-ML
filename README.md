## Skin Cancer Detection with CNN 🧪


This project leverages Convolutional Neural Networks to detect and classify cancer from dermoscopic images. The goal is to assist in early diagnosis by providing an AI-powered model trained on a labeled dataset.

# Project Overview

Skin cancer is among the most common forms of cancer globally. By utilizing deep learning techniques, particularly CNN, this project aims to automate and improve the detection accuracy of skin cancer. The model was trained on large public image datasets from the HAM10000 dataset. Among those images are believed to be a mix of benign and malignant images.

# Tools & Technologies
- Tensorflow
- Python
- Numpy
- Pandas
- Matplotlib
- Google Colab (Used for training with free GPU resources)


# How it works

1. Data Preprocessing:
      - Cleaned labels using Pandas.
      - Normalized image pixel values with NumPy.
      - Split the dataset into training, validation, and test sets.

2. Model Architecture:
      - Custom CNN with Conv2D, MaxPooling, Dropout, and Dense layers.
      - Compiled the model using the Adam optimizer and categorical cross-entropy loss.
      - Utilized the ResNet-50 to improve the model's accuracy.

3. Training:
      - Used TensorFlow’s model.fit() on preprocessed data.
      - Trained for multiple epochs with live performance tracking.
  
4. Prediction
     - Uploads unseen images to classify whether the images are malignant or benign.
  


# Results 📊
  - Achieved ~96% validation accuracy on the balanced dataset.
  - Model successfully identified high-risk skin lesions in test images.
  - Visualized model learning and prediction samples with detailed plots.


# Challenges

1. Imbalanced Dataset
I had to apply data augmentation to reduce bias and avoid skewed predictions.

3. Overfitting
Early in training, the model achieved high training accuracy but poor validation accuracy. I introduced dropout layers, early stopping, and image augmentation to mitigate overfitting.

5. Computational Limitations
Training large CNN models on high-resolution images took up a very long time to process. I used Google Colab to access free GPUs and optimize image size to balance performance and training time.


