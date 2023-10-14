# Collocation Analysis Artifacts

This repository contains the artifacts for the work "An Analysis of Collocation on GPUs for Deep Learning Training". We welcome anybody to reproduce our results.

## Reproduction

We have used the [radT benchmarking framework](https://github.com/Resource-Aware-Data-systems-RAD/radt) to run our tests. Please make sure that you have a working RadT installation by following the guide over at their [repository](https://github.com/Resource-Aware-Data-systems-RAD/radt/tree/master/examples/#readme).

We source the models and training script from [Pytorch Image Models (TIMM)](https://github.com/huggingface/pytorch-image-models). We have included the clone of TIMM that we used in this repository.

The experiments are defined in the `collocation_experiment.csv` file. The experiments can be run via radT, e.g.:

```bash
python -m radt --rerun --epoch 5 --time 99999999 collocation_experiment.csv
```
