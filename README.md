# SpeechEmotionRecognition
This repository contains a complete workflow for building and analyzing a speech recognition system using Python.

1. Data Preparation & Exploration

   DataFrame Creation

     A pandas DataFrame stores two columns:

     speech – full path to the .wav file

     label – the corresponding emotion.

2. Exploratory Analysis

    Class distribution plotted with seaborn.countplot.

3. Audio samples visualized using:

   Waveforms librosa and display.

4. Feature Extraction

    MFCCs (Mel-Frequency Cepstral Coefficients) are the core features.
    
    Each audio clip is:
    
    Loaded at a uniform sampling rate.
    
    Trimmed or padded to a consistent duration (3 s with 0.5 s offset).
    
    Transformed into a 40-dimension MFCC vector.
    
    The mean of the MFCC sequence over time gives a fixed-size 40-element feature vector per file.
    
