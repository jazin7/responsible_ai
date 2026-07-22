# Trustworthiness of Models based on Language

**Authors:** Hannah Buch, Yassine Ajoud

## Overview

This Responsible AI project tests how well a large language model recognizes
literature across languages. The model is shown a short snippet from a book and
has to pick the correct title. If recognition works in English but drops in other languages, 
the abilities of the model do not transfer equally across languages.

## Experiments

All books come from Gutenberg project (HuggingFace dataset
`manu/project_gutenberg`). The model is **Qwen2.5-7B-Instruct**.

- **English:** 100 books
- **German translations:** 23 German translations of English books (`translated_books.csv`)
- **German, French, Italian, Dutch:** 100 native books each

For each language, accuracy is the percentage of the model chosing the right title.

## Files

- `LLM_Gutenberg_Analysis.ipynb`: code, experiments and results
- `translated_books.csv`: manually mapped German/English titles
- `LLM_Gutenberg_Analysis.ipynbf`: project report
- `LLM Literature Analysis.pdf`: presentation slides

## How to run

```
pip install transformers torch accelerate datasets matplotlib
```

Open `LLM_Literature.ipynb` and run all cells up to Accuracy Analysis. Cells after that can then be run, depending on point of interest. (Warning: Especially Noise Analysis needs a lot of time to run). The model is downloaded on the first run.
