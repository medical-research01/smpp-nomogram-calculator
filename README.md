# SMPP Nomogram Calculator

Interactive nomogram calculator for early risk stratification of severe pediatric Mycoplasma pneumoniae pneumonia (SMPP).

## Overview

This tool implements the prediction model described in the associated manuscript. It integrates a serum composite index (derived from CARDS toxin, LC3, and MUC5AC) with clinical parameters (fever duration, CRP, platelet count) to estimate the probability of SMPP.

## Model

- logit(P) = −5.090 + 1.421×MIPI + 0.219×Fever duration + 0.040×CRP + 0.011×PLT
- MIPI = 0.965×Z(CARDS) + 0.941×Z(LC3) + 0.925×Z(MUC5AC)
- P(SMPP) = 1 / (1 + e^(−logit))

## Disclaimer

For research and educational purposes only. This model has not been externally validated and does not replace professional clinical judgment.
