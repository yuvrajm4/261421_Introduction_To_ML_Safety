# Exercise 2 — ODD and Safety Analysis

## Overview

This exercise focuses on defining the Operational Design Domain, also called ODD, and connecting it with safety analysis. The ODD describes the conditions under which a system is expected to operate safely.

## Main Topics

- Operational Design Domain definition
- Environmental and scenario assumptions
- Safety constraints
- Unsafe Control Actions
- Model-level and system-level safety considerations
- Dataset assumptions for autonomous driving scenes

## Key Learning Points

An ML model should not be evaluated only by checking whether it performs well on a test set. It is also important to describe the exact conditions where the model is expected to work.

For example, a driving perception model may be valid only for clear daytime urban scenes with a forward-facing camera. If the system is used in snow, glare, night-time, or unusual traffic situations, this may be outside the original ODD.

## Files

| File | Description |
|---|---|
| `Introduction to ML Safety Ex-2.pdf` | Written solution for Exercise 2 |

## How to Use

Use this exercise as the base for later exercises, especially Exercise 4, where the ODD is checked using k-projection coverage.
