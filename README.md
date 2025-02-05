# TuneTrap-Emotion-Detection-Platform-

About

This repository demonstrates an end-to-end pipeline for real-time Facial emotion recognition application along with reccommending music based on detected emotions. Done in three steps:

1-Face Detection: from the video source using OpenCV.

2-Emotion Recognition: using a model trained by using Mediapipe library.

3-Music Recommendation: Using detected emotion to create a search query on Youtube.

-------------------------------------------------------------------------------------------------------------------------------------

The model is trained for 50 epochs and runs at 87% accuracy.

-----------------------------------------------------------------------------------------------------------------------------------------------

Features

Detection of various emotions like [Sad, Angry, Happy, Neutral, Surprise] 

Detection of various gestures like [Hello, Thumbsup, Nope, Rock] 
![pic2](https://github.com/user-attachments/assets/65f667a8-a78b-4806-b776-eda01a5f07b6)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Dependencies

This project depends on Python and following packages which can be easily installed through requirements.txt file by running the following command: pip install -r requirements.txt

Python 3.9.6

pip 22.1.1

streamlit 1.9.1

streamlit-webrtc 0.37.0

opencv-python 4.5.5.64

mediapipe 0.8.10

----------------------------------------------------------------------------------------------------------------------------

Instructions

Testing Locally

git clone https://github.com/29ananyaseth/TuneTrap-Emotion-Detection-Platform-.

Run pip install -r requirements.txt to install all dependencies.

cd ./TuneTrap-Emotion-Detection-Platform

streamlit run app.py

The app is now running at http://localhost:8501

-> While testing, wait for the model to detect your emotions and click on recommend button to get songs based on a particular emotion

-> Emotion used previously are stored as cache and might cause an error in recommending music, delete detected_emotion.npy file in the directory to resolve this.

-> Recommended music is loaded in next tab as a youtube search query.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Repository Structure

This repository is organised as:

-> app- This file contain the setup of final web app.
-> model- This file contains the trained model.
->Emotion Detection -This folder contains python scripts to train the model.
-> .streamlit- This folder contains configuration files for the streamlit theme in Web App.

------------------------------------------------------------------------------------------------------------------------------
