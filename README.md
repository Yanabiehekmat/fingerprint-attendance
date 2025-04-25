# Fingerprint Attendance System with Siamese Network

This project implements a fingerprint-based attendance system using a Siamese Neural Network with ResNet50V2 as the feature extractor.

## Features
- Identifies fingerprints with ~60% accuracy (can be improved with more data and tuning).
- User registration using 5 fingerprints.
- Fingerprint recognition under 0.5 seconds (with Tesla T4).

## Dataset
The SOCOFing dataset was used and includes real fingerprint images.

## Model
- Architecture: Siamese Network with ResNet50V2 (pretrained)
- Loss: Contrastive Loss
- Optimizer: Adam

## Results
- Achieved accuracy: ~60% on test set
- Model trained on 10 users from SOCOFing dataset

## How to Use
- Train model in `colab`
- Use `register_new_user()` to add a new user
- Use `identify_user()` to recognize a fingerprint
