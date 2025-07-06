# ASL_Recognition_DeepLearning
Real-time American Sign Language recognition using CNN with residual blocks


# 🧠 Real-Time ASL Recognition Using Deep Learning

This project implements a real-time American Sign Language (ASL) alphabet recognition system using a Convolutional Neural Network (CNN) with Residual Blocks.

## 🔍 Overview
- Predicts static ASL hand signs (A–Z) from a live webcam feed.
- Trained on the ASL Alphabet dataset from Kaggle (~87,000 images).
- Real-time inference with temporal smoothing and confidence thresholding.
- Includes performance metrics and visuals from training and prediction phases.

## 🚀 Key Features
- Custom CNN architecture with residual connections
- Early stopping for optimal training efficiency
- Real-time video input and prediction via OpenCV
- Achieved ~97% validation accuracy and ~90% real-time accuracy

## 🖼️ Sample Output
![Prediction Example](./samples/example_prediction.jpg)

## 🧪 Results Summary
| Metric                 | Value         |
|------------------------|---------------|
| Validation Accuracy    | ~97%          |
| Real-Time Accuracy     | ~90%          |
| Inference Speed        | ~30 ms/frame  |
| Avg FPS (on CPU)       | 10–15         |

## 🛠️ Technologies
- Python, TensorFlow, OpenCV
- Jupyter Notebooks (for training & evaluation)
- Webcam for real-time testing

## 📁 Dataset
Kaggle: [ASL Alphabet Dataset](https://www.kaggle.com/datasets/grassknoted/asl-alphabet)

## 🧠 Future Improvements
- Add hand landmark detection
- Explore Transformer-based or attention models
- Expand to dynamic signs and words

## 👤 Author
Alexey Kresin – https://www.linkedin.com/in/alexeykresin/
Email: forkresin@gmail.com

