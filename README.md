# Domain Adaptation with NanoGPT

Small-scale transformer project exploring how a NanoGPT-style language model transfers across very different text domains through zero-shot and few-shot evaluation.

## Overview

This project studies domain adaptation in a compact transformer setting. Instead of treating language modeling as a single-domain problem, it compares how the same model behaves when trained or evaluated across sources with very different token statistics and writing styles.

The repository focuses on:

- training and inspecting a lightweight GPT-style model
- cross-domain zero-shot and few-shot transfer
- analyzing token distributions and entropy changes across domains
- interpreting why adaptation quality changes between corpora

## Why This Project

This is the strongest project in the set for showing direct model-training work. It demonstrates hands-on transformer implementation and evaluation, while also going beyond raw losses to look at what changes in the token space when the model moves between domains.

## Repository Structure

- [notebooks/domain_adaptation_and_interpretability.ipynb](notebooks/domain_adaptation_and_interpretability.ipynb): main project notebook
- [src/nanogpt_model.py](src/nanogpt_model.py): NanoGPT-style model implementation
- [data](data): lightweight corpora used for comparison
- [assets](assets): plots and reference visuals
- [artifacts](artifacts): selected qualitative outputs and logged results

## Tech Stack

- Python
- PyTorch
- Jupyter Notebook
- matplotlib
- NumPy

## Notes

- Heavy checkpoints and full training logs are intentionally excluded from this GitHub-ready version.
- The repository is organized to emphasize the modeling workflow, analysis, and results rather than raw experiment storage.
