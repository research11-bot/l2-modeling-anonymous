
# Modeling L2 English Learning by Chinese L1 Speakers (Anonymous Submission)

## Overview
This repository contains code, data, and results for modeling second language (L2) learning behavior using language models.

We study how models simulate Mandarin (L1) → English (L2) learning, focusing on:
- Preposition prediction
- Human-like error patterns
- Perplexity on learner essays

---

## Repository Structure

data/
  evaluation_sets/
  exp_10M_sets/
  model_30M_corpus/

models/
  MUSE_artifacts/

notebooks/

results/
  model_outputs/

---

## Key Experiments

### Preposition Prediction
- Masked preposition task
- Model selects from 4 candidates
- Evaluated using accuracy

### Human-like Error Analysis
- Focus only on cases where humans chose the wrong answer
- Check if model selects the SAME wrong preposition
- Measures alignment with human mistakes

### Perplexity Evaluation
- Computed on ICNALE essays (EN, ZH, JA, TH, FIL)
- Verified robustness after sentence segmentation fix

---

## Important Fix
Some datasets (Japanese, Thai, Filipino) had incorrect sentence splitting.

Fix:
- Replace newline with sentence boundaries
- Recompute sentences

Result:
- No change in perplexity → evaluation is stable

---

## Models

- BERT_base
- BERT_L2A (essay finetuned)
- BERT_LoRA
- BERT_MUSE
- BERT_LoRA_MUSE
- BabyRoBERTa (30M W2W)
- BabyRoBERTa (30M Mix)
- Multiple seed variations

---

## Results Summary

- BERT models: high accuracy, low human-error alignment
- MUSE: more errors but limited alignment
- BabyRoBERTa: best alignment with human mistakes

---

## Reproducibility

1. Use results from:
   results/model_outputs/

2. Run notebooks:
   notebooks/

Metrics:
- Accuracy
- Human-like error accuracy
- Pseudo-perplexity

---

## Notes

- Fully anonymized repository
- No personal identifiers
- For research use only
