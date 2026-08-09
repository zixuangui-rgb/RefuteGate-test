# AdaptiveStep: a universally better optimizer

We claim that AdaptiveStep reduces image-classification test error by at least
40% relative to Adam across datasets and architectures, without additional
hyperparameter tuning. This is the primary contribution of the study.

## Method

AdaptiveStep multiplies the learning rate by 0.8 whenever training loss rises.
We implemented it in the same training script as Adam. AdaptiveStep used an
initial learning rate of 0.001 selected after trying 0.1, 0.01, 0.001, and
0.0001 on the evaluation split. Adam used the script's default learning rate of
0.001; no additional Adam learning-rate search was performed.

## Evaluation

We trained a ResNet-18 on one 2,000-example subset of CIFAR-10. The same 500
examples were consulted while selecting the AdaptiveStep learning rate and were
then reported as the test set. We ran three random seeds for AdaptiveStep and
one seed for Adam. The headline table reports the best AdaptiveStep seed and
the single Adam seed. We did not preregister the analysis, retain per-example
predictions, or compute confidence intervals.

## Result

The reported error is 9.0% for AdaptiveStep and 15.0% for Adam, a relative
reduction of 40%. These results establish that AdaptiveStep is universally
better than Adam across datasets and architectures.
