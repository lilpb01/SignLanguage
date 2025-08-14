# ASL Sign Language Alphabet Detector

A computer vision project that detects and classifies American Sign Language (ASL) alphabet signs in real time using **Python**, **MediaPipe**, **OpenCV**, and a **Random Forest Classifier** from **scikit-learn**.

## 📌 Features
- Real-time hand tracking with [MediaPipe Hands](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker)
- Landmark-based feature extraction from hand positions
- Classification of ASL alphabet letters (A–Z, excluding J and Z)
- Scripts for **data collection**, **dataset creation**, **model training**, and **inference**

## 📂 Project Structure
├── collect_imgs.py           # Collect hand gesture images

├── create_dataset.py         # Extract features & create dataset

├── data.pickle               # Processed dataset (features & labels)

├── inference_classifier.py   # Real-time ASL detection

├── model.p                   # Trained Random Forest model

├── requirements.txt          # Dependencies

├── train_classifier.py       # Train the classifier

## 📊 Model
- **Algorithm**: Random Forest Classifier 
- **Input Features**: 3D coordinates (x, y, z) of 21 MediaPipe hand landmarks per frame  
- **Training Data**: Collected ASL alphabet gestures 
- **Output**: Predicted ASL alphabet letter  
  
Youtube link: https://youtu.be/e3mMbhMogH8?si=s8nAUx16jKAnBF2U
