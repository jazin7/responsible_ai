# Trustworthiness of Models based on Language

**Authors:** Hannah Buch, Yassine Ajoud

## Overview

This project investigates the **factual correctness** of large language model
answers across **different languages**. The central question is:

- Do models perform equally well when the same questions are asked in different languages?

We focus on **literature-related questions** and compare model accuracy between English and Polish. Both models answer the same 50 simple questions in both languages and we measure accuracy and answer time per language.

## Goals

- Test the correctness of model answers based on language.
- Determine whether models perform equally across different languages.
- Compare accuracy between languages.

## Models

- TinyLlama-1.1B-Chat (Llama family)
- Qwen2.5-1.5B-Instruct (Qwen family)

## Files

- `main.ipynb`: code, experiments and results
- `report.pdf` / `report.tex`: project report

## How to run

```
pip install transformers torch accelerate pandas matplotlib
```

Open `main.ipynb` and run all cells. The two models (about 5 GB) are downloaded on the first run. On a laptop CPU the full run takes around 30 minutes.
