# multiclass_image_classification

Deep Learning-Based Image Classification Model

This project implements a Multiclass Image Classification System using EfficientNetB0 as a feature extractor. The model is trained on a dataset of images categorized into multiple classes, leveraging Transfer Learning, Data Augmentation, and Class Weighting to improve performance.

 Features
✅ Transfer Learning with EfficientNetB0 → Uses a pre-trained EfficientNetB0 model for feature extraction.
✅ Data Augmentation → Applies random cropping, brightness adjustment, contrast enhancement, and flipping to improve generalization.
✅ Class Imbalance Handling → Computes class weights dynamically to balance underrepresented classes.
✅ Optimized Training Strategy → Uses Adam optimizer with Exponential Learning Rate Decay for better convergence.
✅ Regularization & Dropout → Prevents overfitting with L2 regularization and dropout layers.
✅ GPU Acceleration → Runs efficiently using TensorFlow MirroredStrategy for multi-GPU training.

Dataset
The dataset consists of images classified into multiple categories:
Airplanes ✈️
Cars 🚗
Ships 🚢
(Additional classes can be included)
Each image is resized to 128×128 pixels for efficient processing.
Dataset originally from Kaggle: https://www.kaggle.com/datasets/abtabm/multiclassimagedatasetairplanecar

Tech Stack
Framework: TensorFlow / Keras
Model: EfficientNetB0 (Pretrained on ImageNet)
Optimizer: Adam with ExponentialDecay
Dataset Loading: image_dataset_from_directory()
Evaluation Metrics: Accuracy, Loss, Confusion Matrix, Classification Report
Hardware: GPU (via Google Colab)


Model Training & Performance
The model is trained using:
Batch Size: 64
Epochs: 30 (with early stopping)
Learning Rate Decay: 0.0002 → decays by 5% every 500 steps


Visualization:
Training & Validation Accuracy/Loss Plots
Confusion Matrix
Classification Report

Results & Improvements
Validation Accuracy: Achieved up to 56% after fine-tuning.
Future Improvements:
🔹 Hyperparameter tuning for better generalization
🔹 More advanced augmentation techniques
🔹 Fine-tuning EfficientNetB0 further


Contributions
Want to improve this project? Feel free to:

Fork the repository
Make enhancements
Submit a pull request!
