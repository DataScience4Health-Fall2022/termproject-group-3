# TermProject - DS4H 

## Group 3

In this project, we will be implementing a ViT based SOTA model for classifying fundus images from the MuReD dataset.


## Instructions

All the models are derived from the [timm](https://github.com/rwightman/pytorch-image-models) library. Clone down the repository and install the requirements as per the [documentation](https://timm.fast.ai/).

Model training was completed with the library's pretrained models and `train.py` factory parameters. The parameters used for various runs can be found in the [Commands Used.md](commands_used.md) file.

The extra metrics (F1, AUROC, Average Precision, Recall) were all coded on top of `validate.py` from the `timm` library, called `validate_extra.py`. This file functions identically to the original, except now with the extra flag `'--extra-metrics'` which can be set to enable calculation of these metrics using the [`torchmetrics`](https://torchmetrics.readthedocs.io/en/stable/) library. The code that was implemented is `extra_metrics()` function. This does require the `torchmetrics`  dependency to execute, and produces verbose logs with the values as well as specified `.csv` files with the results. 


The sweeps were implemented using Weights & Biases. This was accomplished by creating a copy of `train.py` where the parameters were configured for the training loop. Once connected to wandb, the sweeps were all created and recorded automatically. 

The images of RandAugment, CutMix, and the feature extraction were all coded in their own scripts. 


## Team Members

[Will Romano](https://github.com/romano-w)

Timothy Yang

Tate Toussaint

Scott Dayton
