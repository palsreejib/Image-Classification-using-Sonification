# Audio Conversion & Visualization Utilities

This notebook  contains code for converting images into audio (low-level image sonification via the Griffin-Lim algorithm) and visualizing audio as spectrograms, supporting the Image Sonification project.

## Contents
These utility notebooks implement:

### Grayscale Image to Audio Conversion using the Griffin-Lim algorithm

* Resizes and normalizes images

* Interprets images as magnitude spectrograms

* Reconstructs audio waveforms

* Saves output as .wav files

 ### Spectrogram Visualization

* Loads audio files (.wav)

* Computes STFT and decibel-scaled spectrograms

* Displays using a linear frequency axis for analysis

## Notes
These notebooks are for preprocessing and analysis only; they do not contain model training code.

Ensure the image and audio files are available locally; modify the paths accordingly if necessary.

## How to Use
Open the notebook in Jupyter or VS Code and execute the cells one step at a time.
These tools are useful for preparing sonified datasets and inspecting the quality of the signals.
