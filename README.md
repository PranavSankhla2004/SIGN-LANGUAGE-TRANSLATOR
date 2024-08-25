<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Indian Sign Language Translation Project</title>
</head>
<body>

    <h1>Project Title: Indian Sign Language Translation</h1>

    <h2>Project Description</h2>
    <p>
        This project aims to develop a machine learning model capable of translating Indian Sign Language (ISL) into text or speech, and vice versa. 
        The goal is to bridge the communication gap between the deaf community and the hearing population, enabling more inclusive and accessible interactions. 
        This model will serve as a foundation for a comprehensive mobile application designed to assist deaf and mute students in Gujarat, helping them learn Gujarati through sign language.
    </p>

    <h2>Dataset</h2>
    <ul>
        <li><strong>Source:</strong> <a href="https://www.kaggle.com/datasets/soumyakushwaha/indian-sign-language-dataset">Kaggle ISL Dataset</a></li>
        <li><strong>Content:</strong> 75 videos of different ISL words, each 3 seconds long.</li>
        <li><strong>Format:</strong> Videos (likely in MP4 or similar format)</li>
        <li><strong>Labels:</strong> Textual labels for each video representing the corresponding ISL word.</li>
    </ul>

    <h2>Model Architecture</h2>
    <p><strong>Neural Network Type:</strong> Convolutional Neural Network (CNN) followed by a Long Short-Term Memory (LSTM) network.</p>
    <p><strong>Framework:</strong> TensorFlow or PyTorch.</p>

    <h3>Rationale:</h3>
    <ul>
        <li><strong>CNN:</strong> Effective for extracting spatial features from the video frames, capturing the visual characteristics of the hand gestures.</li>
        <li><strong>LSTM:</strong> Well-suited for handling sequential data, such as the temporal sequence of frames in a video, and understanding the context of the sign.</li>
    </ul>

    <h2>Implementation Details</h2>
    
    <h3>Data Preprocessing:</h3>
    <ol>
        <li><strong>Extract Frames:</strong> Extract frames from the videos.</li>
        <li><strong>Normalize & Resize:</strong> Normalize and resize the frames.</li>
        <li><strong>Label Encoding:</strong> Convert textual labels to numerical representations (e.g., one-hot encoding).</li>
    </ol>

    <h3>Model Training:</h3>
    <ol>
        <li><strong>Dataset Splitting:</strong> Split the dataset into training, validation, and testing sets.</li>
        <li><strong>Training Process:</strong> Train the CNN-LSTM model using an appropriate loss function (e.g., cross-entropy) and optimization algorithm (e.g., Adam).</li>
        <li><strong>Hyperparameter Tuning:</strong> Experiment with different hyperparameters (e.g., learning rate, batch size) to optimize performance.</li>
    </ol>

    <h3>Evaluation:</h3>
    <ol>
        <li><strong>Performance Metrics:</strong> Evaluate the model's performance using metrics such as accuracy, precision, recall, and F1-score.</li>
        <li><strong>Analysis:</strong> Analyze the model's predictions to identify areas for improvement.</li>
    </ol>

    <h2>Current Status</h2>
    <p>
        The initial focus is on preparing the machine learning model, which will serve as the core of the mobile application. 
        Once the model is optimized, it will be integrated into the app for real-time ISL translation.
    </p>

</body>
</html>
