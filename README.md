# SIGN-LANGUAGE-TRANSLATOR
# Project Title: Indian Sign Language Translation

## Project Description
This project aims to develop a machine learning model capable of translating Indian Sign Language (ISL) into text or speech, and vice versa. The goal is to bridge the communication gap between the deaf community and the hearing population, enabling more inclusive and accessible interactions. This model will serve as a foundation for a comprehensive mobile application designed to assist deaf and mute students in Gujarat, helping them learn Gujarati through sign language.

## Dataset
- **Source:** [Kaggle ISL Dataset](https://www.kaggle.com/datasets/soumyakushwaha/indian-sign-language-dataset)
- **Content:** 75 videos of different ISL words, each 3 seconds long.
- **Format:** Videos (likely in MP4 or similar format)
- **Labels:** Textual labels for each video representing the corresponding ISL word.

## Model Architecture
- **Neural Network Type:** Convolutional Neural Network (CNN) followed by a Long Short-Term Memory (LSTM) network.
- **Framework:** TensorFlow or PyTorch.

### Rationale:
- **CNN:** Effective for extracting spatial features from the video frames, capturing the visual characteristics of the hand gestures.
- **LSTM:** Well-suited for handling sequential data, such as the temporal sequence of frames in a video, and understanding the context of the sign.

## Implementation Details

### Data Preprocessing:
1. **Extract Frames:** Extract frames from the videos.
2. **Normalize & Resize:** Normalize and resize the frames.
3. **Label Encoding:** Convert textual labels to numerical representations (e.g., one-hot encoding).

### Model Training:
1. **Dataset Splitting:** Split the dataset into training, validation, and testing sets.
2. **Training Process:** Train the CNN-LSTM model using an appropriate loss function (e.g., cross-entropy) and optimization algorithm (e.g., Adam).
3. **Hyperparameter Tuning:** Experiment with different hyperparameters (e.g., learning rate, batch size) to optimize performance.

### Evaluation:
1. **Performance Metrics:** Evaluate the model's performance using metrics such as accuracy, precision, recall, and F1-score.
2. **Analysis:** Analyze the model's predictions to identify areas for improvement.

## Current Status
The initial focus is on preparing the machine learning model, which will serve as the core of the mobile application. Once the model is optimized, it will be integrated into the app for real-time ISL translation.
