# bio-ai-journey

Public log of my transition into machine learning for biology and longevity.

I learn by building. Every exercise, experiment and project lands here — including the ones that did not work, and the ones where I was the thing that was wrong.

## Log

| Date | What |
|------|------|
| 2026-07-31 | Started. First run of IBM's MAMMAL protein foundation model. |
| 2026-07-31 | Ran the solubility head on insulin B, lysozyme and a synthetic poly-GPP repeat. All three returned the same class, with the highest confidence on the sequence I expected to be least soluble. Read this as a model failure. It was not. |
| 2026-07-31 | Corrected the above. This checkpoint is fine-tuned on DeepSol, which measures soluble expression in E. coli, not solubility in water, so the question I asked was not the one the model answers. Benchmarked it properly on 100 sequences from the labelled DeepSol test set: accuracy 0.77, AUROC 0.86 (TP 32, TN 45, FP 13, FN 10), matching the accuracy reported in the DeepSol paper. Then probed out of distribution: mean confidence on real proteins is 0.788, but a synthetic poly-GPP repeat scores 0.998 and poly-Q 0.976, and amyloid-beta 42 is called soluble at 0.887. The model never abstains, and its confidence carries no information about whether the input resembles anything it was trained on. |

## Current focus

Python fundamentals, working with biological datasets.

## Roadmap

| Stage | Status |
|-------|--------|
| Python and data analysis | in progress |
| Classical ML and deep learning (PyTorch) | planned |
| Transformers and protein language models | planned |
| Project 1 — protein property prediction: fine-tuned foundation model vs ESM-2 baseline | planned |
| Project 2 — zero-shot variant effect prediction | planned |
| Project 3 — single-cell state classification | planned |

## About

Ihor Stanishevskyi, Ukraine.
