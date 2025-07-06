ASL RECOGNITION PROJECT - README
================================

Author: Alexey Kresin
Course: CS552 Deep Learning
Instructor: Qian Cheng
Date: June 28 2025


PROJECT OVERVIEW:
-----------------
This project implements an American Sign Language (ASL) alphabet recognizer using a convolutional neural network (CNN). It includes both a real-time webcam interface and manual image testing.

Initially, a custom dataset was considered, but due to performance and generalization limitations, we switched to a publicly available preprocessed dataset from Kaggle.

The final model uses residual blocks, temporal smoothing, and a confidence threshold to improve accuracy and robustness during real-time inference.


DATASET USED:
-------------
Name: ASL Alphabet
Source: https://www.kaggle.com/datasets/grassknoted/asl-alphabet
Classes: 29 (A–Z, plus "del", "space", "nothing")
Images per class: 3000
Image size: 200x200 (resized internally to 128x128 for real-time inference)

Only letters A-Z were used during evaluation. "del" and "space" were excluded from predictions.


HOW TO USE:
-----------
1. `asl_realtime_predict.py` – Run for real-time hand sign detection via webcam.
2. `check_manual.py` – Run to test static images and show prediction.
3. `train_notebook.ipynb` – Jupyter notebook used to preprocess data, build, and train the model.
4. `asl_model.keras` – Pretrained model file used for prediction.

Ensure your webcam is connected before running the real-time script.


FILES INCLUDED:
---------------
- ASL_Project_Report.pdf
- ASL_Project_Presentation.pptx
- asl_model.keras
- ASL_Code/
  - check_manual.py
  - asl_realtime_predict.py
  - train_notebook.ipynb
- Test_Screenshots/ (examples of model performance)


NOTES:
------
- The model performs best with clean, centered signs.
- Real-time predictions may vary depending on lighting, background, and camera quality.
- Letters A, B, and X showed lower recognition accuracy, as explained in the report.
