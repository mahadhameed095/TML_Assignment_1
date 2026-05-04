# TML 2026 - Task 1: Membership Inference Attack

## Approach
Likelihood Ratio Attack (LiRA) from Carlini et al. (2022) using 64 shadow models trained on random 50% subsets of the public dataset.

## How to reproduce best result

1. Open `solution.ipynb` on Kaggle
2. Enable GPU T4 accelerator (Settings → Accelerator → GPU T4)
3. Add your API key where it says `YOUR_API_KEY_HERE`
4. Run All cells

The notebook handles data downloading, shadow model training (~7 hours), LiRA scoring, and submission automatically.

## Results
- Baseline TPR@5%FPR: ~0.05 (random)
- LiRA with 64 shadow models: 0.056
