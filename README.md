# XLNet with Google Colab TPU

XLNet often needs more GPU RAM than what is available. In addition, the TPU code written by the authors is intended for the TPU instances on Google Cloud Platform. Therefore, I refactored part of the code to adapt the model to the Google Colab TPU.

As an illustration, XLNet is fine-tuned on the annotated Twitter data for medication intake to detect medication intake events. The data comes from the NIH-funded R01 project [SOCIAL MEDIA MINING FOR PHARMACOVIGILANCE](https://projectreporter.nih.gov/project_info_description.cfm?projectnumber=2R01LM011176-06A1) (Project number: 2R01LM011176-06A1).

## Run Environment

The code was run on Google Colab using the free instance of TPU (64 GB RAM). In addition, it requires access to a Google Cloud Storage bucket.

## Requirements

* tabulate
* tensorflow==1.15

## Files

* XLNet_classifier_TPU.ipynb

If you are interested in the data, please contact Graciela Gonzalez-Hernandez (gragon@pennmedicine.upenn.edu) and Haitao Cai (hcai.pku@gmail.com).
* train.tsv
* validation.tsv
* test.tsv

## Pre-trained model

The pre-trained XLNet model will be downloaded when running the Jupyter notebook, if not already present.
