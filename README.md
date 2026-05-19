# 🎧 ML Audio Visualizer

An end-to-end machine learning audio visualizer that transforms music into real-time visual effects based on predicted emotional “mood.” The system processes audio, runs a trained ML model for mood classification, maps outputs through a mood system, and generates dynamic visuals driven by both audio features and model predictions.

---

## 🧠 Overview

This project combines audio signal processing, machine learning, and procedural visualization.

Audio is analyzed in real time, passed into a trained model, converted into a mood state, and used to control visual behavior like color, motion, and shape generation.

---

## ⚙️ Pipeline

Audio Input  
→ Feature Extraction (volume, pitch, tempo, spectral data)  
→ ML Model (mood prediction)  
→ Mood Table Mapping  
→ Visualizer Engine (real-time graphics)

---

## 📁 Project Structure

ml-audio-visualizer/

├── model/  
│   ├── model.py              # ML model architecture  
│   ├── train.py              # Training pipeline  
│   ├── dataset_loader.py     # Data preprocessing  

├── visualizer/  
│   ├── visualizer.py         # Core rendering engine  
│   ├── audio_engine.py       # Audio feature extraction  
│   ├── effects.py            # Mood-based visuals  

├── mood_system/  
│   ├── mood_table.py         # Maps predictions to moods  
│   ├── mood_logic.py         # Mood processing rules  
│   ├── labels.json           # Mood definitions  

├── data/  
│   └── audio datasets / features  

├── main.py                   # Entry point  
└── README.md  

---

## 🧪 Model Training

The model is trained on extracted audio features to classify emotional states (calm, happy, sad, energetic, etc.).

```bash
python model/train.py
