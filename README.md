Flute Sound Recognition and Teaching Kit

📌 Project Overview

Flute Sound Recognition and Teaching Kit is a deep learning-based system designed to classify and analyze flute notes. The project uses a CNN-LSTM hybrid model to process audio recordings, extract features using Mel spectrograms, and predict the played notes along with their duration. This tool aims to assist beginners in learning to play the flute more effectively by providing real-time note detection and feedback.

📂 Dataset

The dataset consists of 140+ samples per note, ensuring robust training.

Audio samples have been collected, labeled, and stored in a structured format.

The dataset is available for download: Download Here

Processed data is stored in .npy format for optimized training.

🛠 Data Preprocessing

The raw audio samples undergo multiple preprocessing steps before being used for training:

Loading & Trimming Audio:

Uses librosa to load .wav files.

Applies librosa.effects.split() to remove silent parts.

Feature Extraction:

Mel Spectrogram Calculation: Converts the time-domain signal into a frequency-based representation.

Amplitude Conversion: Uses librosa.amplitude_to_db() to normalize values.

Spectrogram Storage: Stores extracted features as .npy files for efficient training and retrieval.

🤖 Model Architecture

The project employs a CNN + LSTM hybrid model for optimal performance:

Convolutional Neural Network (CNN): Extracts spatial features from Mel spectrograms.

Long Short-Term Memory (LSTM): Captures sequential dependencies for better temporal understanding.

Accuracy: Achieves 80-90% accuracy on the current dataset.

📥 Installation

Ensure you have the required dependencies installed before running the project.

pip install numpy librosa tensorflow pandas matplotlib

🚀 Training the Model

To start training the model, run:

python train.py

This will load the preprocessed data, train the model, and save the trained weights.

🎵 Usage

To predict flute notes from an audio file:

python predict.py --file path/to/audio.wav

The model will output:

Predicted Note (e.g., Sa, Re, Ga, etc.)

Duration of the Note (in milliseconds)

🔮 Future Improvements

Expand the dataset with more real-world flute recordings.

Real-time Note Detection using optimized inference.

Deploy as a Web/Mobile App for accessibility.

👤 Author

[Rounak sondawale]

Email: [rounaksondawale@gmail.com]

GitHub: [rounaksondawale]
