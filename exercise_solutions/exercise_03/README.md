# Exercise 3 — Dataset Exploration and Object Detection

## Overview

This exercise works with the CARLA dataset and explores the training and test data used for object detection tasks. The notebook loads the dataset from Google Drive, checks the labels, explores class distributions, and prepares the data for binary classification tasks.

## Main Tasks

- Mount Google Drive in Colab
- Load the CARLA train and test folders
- Read the label CSV files
- Inspect the available labels
- Count training and test images
- Analyze class distribution for:
  - pedestrian
  - traffic light
  - vehicle
- Train or evaluate binary object detection models

## Dataset Path

The notebook expects the dataset at:

```text
/content/drive/MyDrive/introduction_to_ml_safety/
```

Expected structure:

```text
introduction_to_ml_safety/
├── train/
│   ├── labels.csv
│   └── rgb-front/
└── test/
    ├── labels.csv
    └── rgb-front/
```

## Files

| File | Description |
|---|---|
| `Introduction To ML Safety Ex-3.pdf` | Written solution for Exercise 3 |
| `Introduction_To_ML_Safety_Ex3.ipynb` | Colab notebook for dataset exploration and model work |

## Main Results

The notebook checks that the train and test folders exist and reports the number of images in each split. It also analyzes the class balance for the selected object labels.

## How to Run

1. Open the notebook in Google Colab.
2. Mount Google Drive.
3. Make sure the dataset is available in the expected folder.
4. Run the cells from top to bottom.

## Notes

The dataset download and unzip commands may be commented out after the first successful run to avoid downloading the same data again.
