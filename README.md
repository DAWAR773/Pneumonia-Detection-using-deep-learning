# Pediatric Chest X-Ray Pneumonia Classification

An educational deep-learning project that classifies pediatric chest X-ray images into **NORMAL** and **PNEUMONIA** using transfer learning with DenseNet-121.

## Features

- Kaggle dataset download and directory validation
- Image preprocessing and data augmentation
- DenseNet-121 transfer learning with class-weighted loss
- Validation-based checkpoint selection
- Held-out test evaluation: accuracy, precision, recall, F1-score, confusion matrix, and ROC-AUC
- Grad-CAM visualization for model explainability
- Optional Gradio interface for interactive image testing
- Image-transformation stress tests

## Run in Google Colab

1. Open the notebook in Google Colab.
2. Select **Runtime → Change runtime type → T4 GPU** (GPU recommended).
3. Run the notebook from top to bottom.
4. When prompted, provide your Kaggle username and API key, or add `KAGGLE_USERNAME` and `KAGGLE_KEY` to Colab Secrets.

The notebook uses the Kaggle dataset `paultimothymooney/chest-xray-pneumonia`. You must have access to the dataset and comply with its terms.

## Main technologies

- Python
- PyTorch and Torchvision
- DenseNet-121
- scikit-learn
- Matplotlib and Seaborn
- OpenCV and Pillow
- Gradio

## Important limitations

This is an educational prototype, not a medical device. It has not been clinically validated and must not be used to diagnose, treat, triage, or make decisions about patients. Dataset performance does not guarantee performance on images from other hospitals, devices, age groups, or populations. Grad-CAM is an explanatory visualization, not proof that the model reasons correctly.

## Suggested future improvements

- Verify patient-level train/validation/test splits to prevent leakage.
- Evaluate on an external dataset from a different institution.
- Report confidence intervals and calibration metrics.
- Add unit tests for preprocessing and inference.
- Pin dependency versions after confirming the notebook runtime.
