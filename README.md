# 🎧 ML Audio Emotion Visualizer

A machine learning–based project built in Google Colab that analyzes audio and generates visual representations driven by predicted emotional state (mood). The project combines audio feature processing, a trained CNN model, and a mood mapping system to transform sound into emotion-based visual outputs.

Developed with Claire Kim, Daniel Chen, Nathaniel Scanlon, and Sohum Walavalkar as part of final project for Art and Machine Learning course at CMU

## 🧠 Overview

This project explores the relationship between audio signals and emotion by:
- Extracting audio features from input sound
- Using a trained CNN model to predict emotional state
- Mapping predictions through a custom mood table system
- Generating visual outputs based on predicted mood

The entire workflow was developed and executed in **Google Colab notebooks**.

---

## 📁 Repository Structure

```text
emotion_pipeline.ipynb            # End-to-end audio → emotion pipeline
MAIN Image_Generator.ipynb        # Generates visuals from mood/audio features
Final_Mood_Table.ipynb            # Finalized mood mapping logic
Copy of Mood_Table.ipynb          # Experimental version of mood mapping system

emotion_model/
├── best_cnn_model.keras          # Trained CNN model for emotion classification
├── label_scaler.pkl              # Label/feature scaler used for normalization
├── config.json                   # Model configuration and parameters
