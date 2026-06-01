# Exercise 4 — ODD Coverage with k-Projection

## Overview

This exercise evaluates how well the test dataset covers the Operational Design Domain defined in earlier work. The main method used is k-projection coverage.

## Main Tasks

- Load the CARLA test labels
- Create ODD-related columns from the test data
- Define ODD dimensions such as:
  - weather
  - lighting
  - camera condition
  - scene type
  - pedestrian presence
  - traffic light presence
  - vehicle presence
- Use k-projection coverage to measure how many combinations are covered
- Report coverage for different values of k

## Files

| File | Description |
|---|---|
| `Introduction To ML Safety Ex-4.pdf` | Written solution for Exercise 4 |
| `Introduction_To_ML_Safety_Ex4.ipynb` | Colab notebook for k-projection ODD coverage |

## External Tool Used

The notebook clones the following helper repository for coverage calculation:

```bash
git clone https://github.com/kkirchheim/odd-coverage.git
```

## Dataset Path

The notebook expects the test data at:

```text
/content/drive/MyDrive/introduction_to_ml_safety/test
```

## Main Idea

k-projection coverage checks whether combinations of ODD factors appear in the test set. For example, for k = 2, it checks pairwise combinations of ODD dimensions.

A low coverage value means the test set does not cover many possible ODD combinations. This is important because a model may look good on the available test data but still be untested in many relevant safety scenarios.

## How to Run

1. Open the notebook in Google Colab.
2. Mount Google Drive.
3. Clone the ODD coverage helper repository.
4. Load the test labels.
5. Run the k-projection coverage calculation.
