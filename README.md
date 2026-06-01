# 261421 Introduction to ML Safety

This repository contains my exercise solutions and code for the course **Introduction to Machine Learning Safety** in SoSe 2026.

The work focuses on practical and theoretical ML safety topics such as operational design domains, dataset exploration, model evaluation, coverage analysis, uncertainty, robustness, and backdoor attacks.

## Repository Structure

```text
261421_Introduction_To_ML_Safety/
├── README.md
├── exercise_solutions/
│   ├── exercise_01/
│   │   └── README.md
│   ├── exercise_02/
│   │   └── README.md
│   ├── exercise_03/
│   │   └── README.md
│   ├── exercise_04/
│   │   └── README.md
│   └── exercise_05/
│       └── README.md
```

## Exercises

| Exercise | Topic | Content |
|---|---|---|
| Exercise 1 | ML Safety Basics | Introductory safety concepts, risk levels, and safety thinking |
| Exercise 2 | ODD and Safety Analysis | Operational Design Domain, hazards, constraints, and safety requirements |
| Exercise 3 | Dataset Exploration and Object Detection | CARLA dataset loading, label exploration, model training, and evaluation |
| Exercise 4 | ODD Coverage | k-projection coverage analysis for the defined ODD |
| Exercise 5 | Robustness, Calibration, and Backdoor Attack | Temperature scaling, confidence thresholding, trigger injection, poisoning, and ASR |

## Environment

Most coding exercises are implemented in **Google Colab** using Python and PyTorch.

Main libraries used:

```text
pandas
numpy
matplotlib
Pillow
torch
torchvision
scikit-learn
```

For Colab execution, the dataset is expected under:

```text
/content/drive/MyDrive/introduction_to_ml_safety/
```

## Notes

This repository is intended for course submission and learning purposes. The explanations are written in a simple way so that the reasoning behind each solution is easy to follow.
