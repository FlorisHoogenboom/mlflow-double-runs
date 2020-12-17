# mlflow-double-runs
This repository contains some minimal examples to reproduce [Issue 3787](https://github.com/mlflow/mlflow/issues/3787) in mlflow.

To run this experiment use the following command
```bash
$ EXPORT MLFLOW_BACKEND_URI=databricks
$ mlflow run . -e train -b databricks --backend-config ./train-cluster-spec.json --experiment-id {your experiment id}
```