# CNN Deep Learning Projects

Three CNN-based image classification projects, each built with 4 convolutional layers, batch normalization, and dropout for regularization.

> All notebooks have been executed — outputs (accuracy, training curves, confusion matrix) are saved inline. Open any `.ipynb` file above to view results directly on GitHub.

## Projects

| Project | Description | Test Accuracy |
|---|---|---|
| [CIFAR-10 Classification](./01_CIFAR10_Classification.ipynb) | 10-class image classification (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck) | ~84% |
| [LFW Face Recognition](./02_LFW_Face_Recognition.ipynb) | Identifies the most photographed individuals in the Labeled Faces in the Wild dataset | ~81% |
| [MRI Brain Tumor Classification](./03_MRI_Brain_Tumor_Classification.ipynb) | Classifies brain MRI scans into glioma, meningioma, pituitary tumor, or no tumor | ~89% |

## Requirements

- tensorflow
- scikit-learn
- matplotlib
- seaborn
- numpy

## Datasets

- **CIFAR-10** — loaded automatically via `tensorflow.keras.datasets`
- **LFW** — loaded automatically via `sklearn.datasets.fetch_lfw_people`
- **Brain Tumor MRI** — must be downloaded separately from [Kaggle](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset) to re-run notebook 3. Outputs are already included in the notebook if you just want to view results.

## Architecture Summary

Each project uses a CNN with:
- 4 convolutional layers (Conv2D + BatchNormalization + MaxPooling)
- Dropout for regularization
- Dense layers for final classification
- Trained and evaluated with accuracy/loss curves and (for the MRI project) a confusion matrix and classification report
