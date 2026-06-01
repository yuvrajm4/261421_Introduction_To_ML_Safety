# Exercise 5 — Calibration, Thresholding, and Backdoor Attack

## Overview

This exercise studies model confidence, robustness, and backdoor attacks on the pedestrian detector. It includes temperature scaling, confidence threshold analysis, trigger injection, data poisoning, retraining, and attack evaluation.

## Main Tasks

- Load the trained pedestrian detector
- Apply temperature scaling to model logits
- Compare accuracy for different temperature values
- Study the effect of confidence thresholds
- Implement a trigger function
- Poison a fraction of pedestrian-positive training images
- Flip poisoned labels from pedestrian present to pedestrian absent
- Retrain the model on poisoned data
- Evaluate:
  - clean recall
  - attack success rate, also called ASR

## Files

| File | Description |
|---|---|
| `Introduction To ML Safety Ex-5.pdf` | Written solution for Exercise 5 |
| `Introduction_To_ML_Safety_Ex5.ipynb` | Colab notebook for temperature scaling and backdoor attack evaluation |

## Dataset and Model Paths

The notebook expects the dataset and trained models under:

```text
/content/drive/MyDrive/introduction_to_ml_safety/
```

Example model directory:

```text
/content/drive/MyDrive/introduction_to_ml_safety/trained_models/
```

Expected model file:

```text
pedestrian_detector.pth
```

## Trigger Description

The backdoor trigger is implemented as a small bright colored square placed on the image. Images with this trigger are used to poison part of the training data.

## Important Metrics

| Metric | Meaning |
|---|---|
| Clean Recall | How well the model detects pedestrians on normal test images |
| Attack Success Rate | Fraction of triggered pedestrian images classified as no pedestrian |

## Main Idea

A backdoor attack can make a model behave normally on clean images but fail when a specific trigger is present. This is dangerous because normal test accuracy may not reveal the hidden failure behaviour.

## How to Run

1. Open the notebook in Google Colab.
2. Mount Google Drive.
3. Check that the test data and trained model files exist.
4. Run the temperature scaling evaluation.
5. Run the trigger and poisoning steps.
6. Evaluate clean recall and attack success rate.
