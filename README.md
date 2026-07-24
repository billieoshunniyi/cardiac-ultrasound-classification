# Computer Vision: Cardiac Ultrasound Image Classification

## Overview
A three-experiment computer vision project classifying cardiac ultrasound 
images using progressively advanced deep learning techniques. Built as part 
of MSc Data Science coursework at Robert Gordon University, the project 
demonstrates a clear learning arc from classical machine learning through 
to transfer learning with explainability.

## Experiments

### Experiment 1: Heart vs Non-Heart Classification
- **Task:** Binary classification of heart vs non-heart ultrasound images
- **Methods:** kNN and SVM on flattened pixel arrays (128x128)
- **Result:** 100% accuracy — correctly attributed to high visual 
  distinctiveness between classes rather than model complexity
- **Key insight:** Strong baseline performance doesn't always indicate 
  a hard problem — understanding why a model performs well is as 
  important as the result itself

### Experiment 2: Mitral Valve State Classification
- **Task:** Open vs closed mitral valve classification — a significantly 
  harder intra-class task with subtle visual differences
- **Methods:** Custom CNN (Conv2D → MaxPool → Dense layers) with 
  5-fold cross-validation
- **Evaluation:** Accuracy, AUC-ROC, confusion matrix
- **Key insight:** Deep learning necessary when classical methods 
  insufficient for subtle intra-class variation

### Experiment 3: Transfer Learning with Explainability
- **Task:** Enhanced cardiac classification using pre-trained architecture
- **Methods:** MobileNetV2 transfer learning with data augmentation
- **Explainability:** Grad-CAM visualisations highlighting model attention 
  on cardiac structures
- **Result:** A-grade with excellent feedback
- **Key insight:** Explainability is essential in medical imaging — 
  knowing where a model looks is as important as what it predicts

## Tools & Libraries
Python · TensorFlow · Keras · scikit-learn · OpenCV · NumPy · 
matplotlib · Grad-CAM

## Methods Summary
- Classical ML: kNN, SVM
- Deep Learning: Custom CNN, MobileNetV2 transfer learning
- Data augmentation for improved generalisation
- Cross-validation for robust evaluation
- Grad-CAM for visual explainability

## Business Application
Medical image classification systems can support clinical decision-making 
by providing fast, consistent preliminary analysis of diagnostic images. 
Explainability methods like Grad-CAM are critical for building clinician 
trust in AI-assisted diagnosis by making model decisions interpretable 
and auditable.
