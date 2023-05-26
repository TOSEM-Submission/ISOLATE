# RTAnomaly
![](https://img.shields.io/badge/version-1.0-blue.svg) 
![](https://img.shields.io/badge/language-python-orange.svg)

Here is the repository for ASE submission "Correlation-Aware Performance Issue Identification in Cloud Service Systems". 

## Overview

The following figure shows the overview of our framework RTAnomaly, an automated method for detecting performance anomalies. RTAnomaly consists of two main parts: the relational-temporal embedding part and the anomaly detection with LC-VAE part. The relational-temporal embedding part captures relational and temporal patterns from the original metrics by employing graph attention to extract correlations among metrics and capturing temporal dependencies through GRU and temporal convolution. The anomaly detection part utilizes a label-conditional-VAE (LC-VAE) to distinguish anomalies from normal patterns. 

![RTAnomaly](https://github.com/ASE-Submission/RTAnomaly/assets/131580646/e6a21e32-d5bf-49c4-9e48-18f124f4083e)

## Datasets

We only put one sample of our industrial dataset and SMD dataset here (due to limit of space). However, upon acceptance of this work, we will release all datasets used in our study, including raw data and all labels, and any other relevant materials necessary for replication and analysis of our findings.

## Requirements

Python $\geq$ 3.8 is needed. Besides, the environment can be built by:
```pip install -r requirements.txt```

## Run the code
Cd to the current working directory and simply run:
```python train.py```
