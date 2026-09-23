# Music Classification App

This repository contains a MATLAB-based application developed for classifying music and audio signals. It was created as a term project for the **Signals and Systems (Sinyaller ve Sistemler)** course.

## Overview
The application provides an interactive **Graphical User Interface (GUI)** built using **MATLAB App Designer**. It allows users to load an audio file (`.wav`), load a pre-trained machine learning model (`.mat`), and visualize the audio signal's characteristics through a spectrogram.

## Features & Capabilities
- **WAV File Import**: Easily browse and select `.wav` audio files to be processed.
- **Pre-Trained Model Loading**: Supports loading custom `.mat` files containing trained machine learning models (e.g., SVM, KNN, Decision Trees, Neural Networks) for genre prediction.
- **Audio Signal Processing**: Calculates the short-time Fourier transform (STFT) of the loaded audio signal to generate its frequency representation over time.
- **Log-Spectrogram Visualization**: Dynamically displays a 2D Log-Spectrogram of the audio file, plotting Frequency (Hz) against Time (s) with an intensity color bar.
- **Model Selection Interface**: Includes a dropdown menu to select among various classification algorithms (e.g., Fine Tree, Linear SVM, Fine KNN, Boosted Trees, Neural Networks).

## GUI Components
- **Select WAV File**: Reads the selected audio and extracts raw audio data and sampling frequency.
- **Load Model**: Prompts the user to load a `.mat` workspace variable representing the trained network/model.
- **Predict Genre**: Analyzes the audio, generates the spectrogram, and (based on the loaded model) prepares the data for classification.
- **Spectrogram View**: An interactive axis area to visualize the signal's frequency components.

## Prerequisites
To run this application, you will need:
- **MATLAB** (R2018a or newer is recommended for App Designer support)
- Signal Processing Toolbox (required for the `spectrogram` function)
- Audio Toolbox (recommended for audio I/O operations)
- Statistics and Machine Learning Toolbox / Deep Learning Toolbox (depending on the `.mat` models used for classification)

## How to Run
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/zeynepertas/Music-Classification-App.git
   ```
2. Open MATLAB.
3. Navigate to the `MusicClassificationApp` directory within the project folder.
4. Double-click on `app2.mlapp` to open it in the App Designer, and click the **Run** button.
5. Alternatively, you can run the app directly from the MATLAB command window by typing:
   ```matlab
   app2
   ```

## Usage Instructions
1. Click **Select WAV file** and choose a music sample.
2. Click **Load Model** and select your trained `.mat` model file.
3. Click **Predict Genre** to generate the spectrogram and run the prediction.

## Author
**Zeynep Sude Ertaş** - 211015054
