# Bird-Species-Identifier
This project presents a multi-modal deep learning system designed to identify bird species from both audio recordings of bird calls and images of birds. Developed with a focus on accuracy and user accessibility, the system combines advanced machine learning models with a user-friendly web interface.

Key Features:
Multi-Modal Identification: Accurately classifies bird species using distinct inputs:
Audio Recognition: Identifies birds based on their calls and vocalizations.
Image Classification: Recognizes birds from photographs.
Advanced Feature Extraction:
Audio: Employs librosa to extract sophisticated features such as Mel-frequency cepstral coefficients (MFCCs), Chroma, Spectral Contrast, Tonnetz, and Spectral Bandwidth.
Images: Utilizes image preprocessing techniques including rescaling and data augmentation, and leverages a pre-trained VGG16 model for robust feature learning.
Deep Learning Models:
Audio Model: Features an ensemble of deep learning architectures, including a Convolutional Recurrent Neural Network (CRNN) with an attention mechanism and a standard Convolutional Neural Network (CNN), trained for bird sound classification.
Image Model: Utilizes a fine-tuned Convolutional Neural Network built upon the VGG16 architecture, benefiting from transfer learning on a large image dataset.
Ensemble Learning (Audio): Enhances prediction robustness and accuracy for audio classification by combining the outputs of multiple audio models through an averaging ensemble method.
Integrated Knowledge Base: Enriches identification results by fetching and displaying relevant information about the identified bird species from Wikipedia, including summaries, scientific names, and additional images.
User-Friendly Web Interface (Flask): Provides an intuitive web application built with Flask, allowing users to easily:
Upload audio files (WAV, MP3, FLAC, WebM, Ogg) or images (PNG, JPG, JPEG, WebP).
Record audio directly from a microphone or capture images using a camera.
View detailed prediction results and supplementary information in a clear format.
Technologies Used:
Backend: Python, Flask
Machine Learning: TensorFlow, Keras, NumPy
Audio Processing: Librosa, ffmpeg (for WebM conversion)
Image Processing: Pillow (PIL)
Data Handling: Scikit-learn (LabelEncoder), json, pickle
External API: Wikipedia API wrapper
