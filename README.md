# 🐦 Bird Species Identifier: Audio & Image-Based
This project is a bird species identification system that can predict bird species using either bird calls (audio recordings) or bird images. It integrates deep learning models with a Flask web app interface, providing additional insights such as scientific classification and Wikipedia information.

## 🔍 Features 

- 🎙️ Audio Classification
Detects bird species from recorded bird calls or uploaded audio files using a CRNN-CNN ensemble trained on Mel-frequency and spectral audio features.

* 📸 Image Classification
Identifies bird species from images using a fine-tuned VGG16 CNN model.

+ 🌐 Wikipedia Integration
Automatically fetches Wikipedia summary, image, and link for the predicted species.

- 🧠 Ensemble Learning
Audio model includes both CRNN and CNN architectures combined into an ensemble to boost accuracy.

- 💡 Robust Preprocessing
Handles short audio clips, converts webm audio to WAV using FFmpeg, and ensures padded/truncated feature vectors.

- 🖼️ Visual Training Summary
Training accuracy/loss plots for image model saved automatically.

## 🏗️ Tech Stack
- Frontend: HTML5, CSS3, JavaScript, Bootstrap 5

- Backend: Flask (Python)

- ML/DL Frameworks: TensorFlow / Keras

- Audio Processing: Librosa

- Image Model: VGG16 (transfer learning)

- Audio Model: CRNN + CNN Ensemble with Attention

- Storage: Local file uploads with validation

- Extra: Wikipedia API, FFmpeg integration, CORS support  

## 🧪 Model Training
- Audio_model_training.py: Builds and trains an ensemble of CRNN and CNN on MFCC + spectral audio features.

- Image_model_training.py: Fine-tunes a VGG16 model on labeled bird image datasets.
