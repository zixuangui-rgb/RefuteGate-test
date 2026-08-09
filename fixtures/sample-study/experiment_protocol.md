# Experiment record

- Dataset: one fixed 2,000-example CIFAR-10 subset.
- Evaluation set: 500 examples reused for hyperparameter selection and reporting.
- Architecture: ResNet-18 only.
- AdaptiveStep seeds: 1, 2, 3.
- Adam seeds: 1 only.
- Reported comparison: best AdaptiveStep seed versus the only Adam seed.
- Stored artifacts: aggregate error rates only; no checkpoints or predictions.
- Confirmatory holdout: none.
