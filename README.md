# L2 Preposition Modeling (Anonymous)

This repository contains code, data, and results for experiments on second language (L2) preposition modeling.

## Overview

The goal of this project is to evaluate how different language models predict English prepositions in context, and to analyze whether model behavior aligns with human learner patterns.

The experiments focus on:
- Masked preposition prediction
- Human-like error analysis
- Perplexity evaluation on learner corpora

---

## Repository Structure

notebooks/              # Evaluation and analysis notebooks
data/
  evaluation_sets/      # Cleaned learner corpora and evaluation data
results/
  model_outputs/        # Model prediction outputs (normalized)

---

## Data

The evaluation data includes learner corpora from multiple L1 backgrounds:
Chinese, Japanese, Korean, Thai, Filipino, Urdu, and native English.

---

## Model Outputs

The results/model_outputs/ folder contains normalized probability outputs for multiple models including:
Base BERT, BERT variants (CSEE, LoRA, MUSE), and BabyRoBERTa models with different training settings.

---

## Experiments

1. Preposition Prediction
Models predict masked prepositions in sentences.

2. Human-like Error Analysis
We evaluate whether models select the same incorrect prepositions as human learners.

3. Perplexity Evaluation
Pseudo-perplexity is computed on learner corpora. Sentence segmentation fixes were tested and did not affect results.

---

## Notes

- Notebooks are cleaned (no outputs, no personal paths)
- Paths are relative to repository
- Model weights are not included

---

## Reproducibility

Use the data and notebooks provided to reproduce results.

---

## Disclaimer

This repository is anonymized for review purposes.
