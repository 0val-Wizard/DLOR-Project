# DLOR-Project
Deep Learning and Object Recognition (DLOR) it introduces students to the fundamental principles of deep learning and how it is applied to a collection of computer vision tasks to implement object recognition. It covers the concepts and architecture of convolutional neural networks such as the various layers within, and the hyperparameters involved

# Deep Learning Pipeline Summary
## 1. Dataset Preparation
- Mounted Google Drive to access data.
- Loaded dataset(s) into Pandas.
- Shuffled the combined dataset to avoid order bias.
- Installed dependencies (kaggle, tensorflow, keras, umap-learn).

## 2. Dataset Exploration & Visualization
- Checked dataset info, head, summary statistics.
- Verified data types and null values.
- Counted unique labels and samples per class.
- Checked for missing values and duplicates.
- Plotted class distribution.
- Examined random samples of images and computed pixel statistics.

## 3. Data Preprocessing & Splitting
- Removed duplicate entries.
- Defined features (X) and labels (y).
- Split into training, validation, and test sets.
- Reshaped image arrays for model compatibility.
- Normalized pixel values (scaling).
- One-hot encoded categorical labels using to_categorical.
- Set random seeds for reproducibility.
- Used ImageDataGenerator for data augmentation.

## 4. Model Architecture & Training
- Built models with TensorFlow/Keras (layers, models, regularizers).
- Implemented an autoencoder for feature extraction & denoising:
- Encoder → compressed latent representation.
- Decoder → reconstructed input image.
- Displayed model summary of encoder, decoder, and autoencoder.
- Trained model with:
- Early stopping callbacks to prevent overfitting.
- Monitored training & validation loss/accuracy.
- Visualized training curves (loss & accuracy vs. epochs).

## 5. Feature Engineering & Dimensionality Reduction
- Applied UMAP (Uniform Manifold Approximation and Projection) for visualization of latent features.
- Extracted encoded representations from the trained autoencoder.
- Used these low-dimensional embeddings for clustering or classification experiments.

## 6. Evaluation
- Verified preprocessing and data splits consistency.
- Evaluated training vs. validation performance.
- Inspected reconstruction quality of autoencoder.
- Compared model’s learned representations against raw features.

## 7. Key Outcomes
- Cleaned & balanced dataset ready for ML/DL.
- Autoencoder successfully reduced input dimensionality while preserving key structure.
- Encoded features prepared for downstream tasks (classification, anomaly detection, visualization).
- Pipeline supports scalability with TensorFlow and visualization with UMAP.

## End-to-End Workflow

Raw data → Preprocessing → Train/Val/Test split → Autoencoder (Encoder/Decoder) → Feature extraction → UMAP visualization → Model evaluation.
