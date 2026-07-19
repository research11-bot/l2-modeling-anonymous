# Modeling Second Language Learning Through a Behavioral Lens

## Overview
This repository contains code, training data, evaluation data, and results for an anonymous paper submission on modeling Mandarin Chinese (L1) to English (L2) learning using BabyRoBERTa-based models.

The final study compares six models:

- Baby_EN
- Baby_L2E
- Baby_MUSE
- Baby_W2W-ZH
- Baby_W2W-Mix
- Baby_EN-ZH

The models are evaluated using:

- Essay pseudo-perplexity
- Preposition selection based on Mandarin L1 learner behavior
- BLiMP grammatical competence evaluation

## Main Notebooks

- `chinese_translation_final_1.ipynb` — Mandarin-to-English word-to-word translation pipeline
- `model_training_evaluation.ipynb` — model training and evaluation workflow

## Data

Training data is available in:

`data/training_data/`

Evaluation data is available in:

`data/evaluation_sets/`

Large training corpora are stored using Git LFS.

## Final Results

Final paper results are available in:

`results/final_results/`

This includes:

- BLiMP detailed results
- BLiMP summary
- preposition evaluation results
- pseudo-perplexity results

## Anonymous Submission

This repository is provided as supplementary material for anonymous peer review.
Author-identifying information has intentionally been omitted.
