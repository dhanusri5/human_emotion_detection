Human Emotion Detection (Audio + Facial Expressions)
-------------------------------------------------------

A multimodal deep learning system that predicts human emotions using speech and facial images. The project combines audio-based and image-based models and merges their embeddings to produce a final emotion classification.

Features
-----------

Emotion detection from voice recordings

Emotion detection from facial expression images

Multimodal fusion model (audio + image)

FastAPI backend for predictions

Simple HTML UI for uploading audio/images

Works fully in Google Colab or local environment

Problem Summary
----------------------
Humans express emotions through voice tone, pitch, and facial expressions.
Traditional systems struggle because of noise, lighting variations, and diverse expressions.

This project predicts emotions such as:
----------
Happy, Sad, Angry, Fearful, Surprised, Neutral

using both speech and facial inputs for improved accuracy.

Datasets
--------
RAVDESS — Audio Speech Dataset
---
1440 speech files

8 emotion classes

Preprocessing includes:
--
MFCC extraction

Mel Spectrogram

Chroma features

Normalization & trimming

FER2013 — Facial Expression Dataset
----
35,887 images (48×48 grayscale)

7 emotion classes

Preprocessing includes:
--
Resize

Normalization

Augmentation (rotation, flip, brightness)

Model Architecture
---
Audio Emotion Model
--

1D CNN or LSTM

Input features: MFCC, Mel-spectrogram, Chroma

Output: Audio emotion embedding

Image Emotion Model
---
2D CNN or Transfer Learning (VGG16/ResNet)

Input: 48×48 facial images

Output: Image emotion embedding

Multimodal Fusion Model
----
Concatenates audio + image embeddings

Fully connected layers

Softmax for final emotion prediction

Tech Stack
--
Python

TensorFlow / Keras

Librosa

OpenCV

NumPy, Pandas

FastAPI (backend)

HTML, CSS, JS (UI)

Google Colab

Expected Output
----
Final predicted emotion label

Confidence score

Option to run audio-only, image-only, or multimodal prediction

Future Scope
----
Real-time webcam + microphone emotion detection

Support for continuous emotion tracking

Deployment as a mobile app or API service

Extension to body-gesture and biometric signals# human_emotion_detection
