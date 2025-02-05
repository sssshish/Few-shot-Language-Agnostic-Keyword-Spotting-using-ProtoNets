# Multi-Model Deep Learning Architecture for Keyword Spotting

This project aims to develop an advanced deep learning-based system for keyword spotting in speech audio. The system is built using a multi-model architecture that incorporates various state-of-the-art techniques to handle keyword detection efficiently, even in low-resource or language-agnostic scenarios.

## Proposed Solution

The proposed solution integrates the following key components:

- **Wav2Vec 2.0 (Transformer Model):** This model specializes in speech tasks and is leveraged to handle keyword spotting with its robust performance in various speech recognition tasks. The use of Multi-Head Attention (MHA) mechanisms in Wav2Vec 2.0 makes it especially effective in keyword detection.
  
- **CNN-LSTM Hybrid Architecture:** The hybrid model uses Convolutional Neural Networks (CNNs) combined with Long Short-Term Memory (LSTM) units. This helps the system capture both local (spatial) and temporal dependencies in audio data, which is crucial for keyword detection in speech.

- **Meta-Learning with MAML (Model-Agnostic Meta-Learning):** MAML is used to enable few-shot learning, making the model capable of adapting to new keywords with minimal data. This technique is designed to generalize well for language-agnostic keyword spotting tasks, reducing the need for large amounts of labeled training data.

- **Prototypical Networks:** These networks are used for efficient few-shot classification, allowing the model to recognize new keywords based on a few examples and improve the performance in low-data environments.

## Dataset

The primary dataset used for training the model is the **Mozilla Common Voice** dataset, which was provided during the hackathon. The dataset includes a wide variety of audio clips in different languages, making it suitable for training a language-agnostic keyword spotting system.

## Architecture

![image](https://github.com/user-attachments/assets/5410ae4c-18c4-4408-91d6-616cbea22539)

## Results

The model outputs a list of detected keywords in the audio file, along with their timestamps. This can be further improved by fine-tuning the model.

![image](https://github.com/user-attachments/assets/a214b037-f6d6-47ea-ac64-a8326880636f)

