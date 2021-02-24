# Argo + Optuna hyperparameter optimization example

This shows how to perform hyperparameter optimization via [Argo Workflows & Pipelines](https://argoproj.github.io/projects/argo/) and [Optuna](https://optuna.org) by an example based on XGBoost.

Hyperparameter optimization is eiter done within a single container per parallel execution via
```
argo submit argo/hyperparameter-tuner-optuna-level.yaml
```
or with new containers for each training run via
```
argo submit argo/hyperparameter-tuner-argo-level.yaml
```