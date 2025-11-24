# Face Recognition System

This repository contains a compact implementation of a face recognition pipeline for video data. It includes face detection using MTCNN, template-matching–based tracking, face alignment, deep embedding extraction with a pre-trained FaceNet model, and both closed-set and open-set identification. Unsupervised person re-identification is supported through k-means clustering, and evaluation tools are provided for DIR curve analysis.

## Features
- Face detection, alignment, and tracking
- Deep feature extraction (128-D FaceNet embeddings)
- k-NN identification with probability and distance outputs
- Open-set recognition using thresholding
- k-means clustering for unsupervised grouping
- DIR curve and evaluation scripts

## Files
- face_detector.py — detection and tracking
- face_recognition.py — embeddings and recognition logic
- classifier.py — k-NN classifier
- evaluation.py, dir_curve.py — evaluation tools
- training.py, test.py — gallery creation and video recognition
- convergence/ — clustering outputs

## Installation
pip install -r requirements.txt

## Usage
python training.py
python test.py
python dir_curve.py

## Reference
Based on instructional material from the Pattern Recognition Lab (FAU).
