# Flute Sound Recognition and Teaching Kit Using CNN-LSTM

## 📌 Project Overview

The **Flute Sound Recognition and Teaching Kit** is a deep learning-based system designed to classify and analyze flute notes. The project uses a **CNN-LSTM hybrid model** to process audio recordings, extract features using Mel spectrograms, and predict the played notes along with their duration. This tool aims to assist beginners in learning to play the flute more effectively by providing real-time note detection and feedback.

## 📂 Dataset

- The dataset consists of **140+ samples per note**, ensuring robust training.
- Audio samples have been collected, labeled, and stored in a structured format.
- The dataset is available for download: **[Download Here](#)**
- Processed data is stored in `.npy` format for optimized training.

## 🛠 Data Preprocessing

The raw audio samples undergo multiple preprocessing steps before being used for training:

### Loading & Trimming Audio
- Uses `librosa` to load `.wav` files.
- Applies `librosa.effects.trim()` to remove silent parts.

### Feature Extraction
- **Mel Spectrogram Calculation**: Converts the time-domain signal into a frequency-based representation.
- **Amplitude Conversion**: Uses `librosa.amplitude_to_db()` to normalize values.
- **Spectrogram Storage**: Stores extracted features as `.npy` files for efficient training and retrieval.

## 🤖 Model Architecture

The project employs a **CNN + LSTM hybrid model** for optimal performance:
- **Convolutional Neural Network (CNN)**: Extracts spatial features from Mel spectrograms.
- **Long Short-Term Memory (LSTM)**: Captures sequential dependencies for better temporal understanding.
- **Accuracy**: Achieves **80-90% accuracy** on the current dataset.

## 📥 Installation

Ensure you have the required dependencies installed before running the project.

```bash
pip install numpy librosa tensorflow pandas matplotlib
