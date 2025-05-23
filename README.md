## Plant Disease Detection System (PDDS)
This project is a deep learning-based system for detecting plant diseases from leaf images using a Convolutional Neural Network (CNN). It uses TensorFlow and Keras to train a model on an augmented dataset of plant diseases and includes a simple Flask web app interface for predictions.

# Features
1. Trains a CNN model on a dataset of 38 plant disease classes
2. Uses data augmentation for improved generalization
3. Evaluates model with accuracy, precision, and recall
4. Visualizes training performance
5. Includes a Flask-based web app for live image-based predictions
6. Supports deployment via Ngrok for remote access

# Dataset
The dataset used is an augmented version of a public plant disease dataset, structured into training and validation directories.

# Model Architecture
1. 4 Convolutional layers
2. 3 MaxPooling layers
3. 2 Dense layers + Softmax output layer
4. Dropout (conceptually included, though not activated in code)
5. Categorical cross-entropy loss with Adam optimizer

# Evaluation Metrics
1. Accuracy
2. Precision
3. Recall

# Web App
A Flask app is provided to allow users to upload leaf images and receive disease predictions. The app is exposed to the internet using Pyngrok.
- How to Run
1. Clone the repository and set up the environment.
2. Extract the dataset to the specified folder.
3. Train the model (`plant_disease_detection.py`).
4. Launch the web app using Flask and Ngrok.
5. Access the app via the public Ngrok URL.

# Dependencies
1. TensorFlow
2. NumPy
3. Matplotlib
4. OpenCV
5. Flask
6. Pyngrok

# Model Output
The trained model is saved as `PDDS.keras` for future predictions.
