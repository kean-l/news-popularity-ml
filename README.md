# Online News Popularity — Predicting Virality

Predicting whether a news article will become popular, from its content and
metadata, to support a target of lifting advertising revenue by ~5%.

## Overview
Final group project (3 members) for UvA Business Analytics — graded 10/10.
We trained classifiers on a ~2-year, ~40,000-article dataset to flag which
articles would go viral, then analysed which features drive popularity.

## Tech
Python · scikit-learn · pandas · NumPy

## What I did
- Handled severe class imbalance (~75% non-popular): set the popularity
  threshold with K-means, then optimised for F1 rather than accuracy.
- Benchmarked logistic regression, random forest, AdaBoost, and histogram
  gradient boosting; the gradient-boosting model performed best.
- Tuned the precision–recall trade-off (final recall 0.68, AUC 0.72) and used
  permutation importance to identify keyword strength as the top predictor.

## Notes
Models are intentionally evaluated honestly on a hard, imbalanced problem —
the focus was rigorous methodology over chasing a headline accuracy number.
