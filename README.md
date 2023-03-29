# TSMC - Temporal and Spatial Micro-Clustering
Temporal and spatial micro-clustering of trajectory process data, based on the method of TADE - Temporal Activity Density Estimation.

# Table of Contents
* [Setup](#setup)
* [Use Instructions](#use-instructions)
* [Description](#description)
* [Modules](#modules)
* [Others](#others)

## Setup

### Setup Virtual Environment
```
!git init
!git clone https://github.com/qishangxin/TSMC.git
```
### Requirements
Install requirements.txt <br />
```
pip install -r requirements.txt
```
Install setup.py <br />
```
python setup.py install
```

## Use Instructions

1. In pre-TADE.ipynb in the notebooks folder, configure the location of prozess_model and telegramme_logs
2. Run pre-TADE.ipynb to create merged_log.csv file and detect numerical and sequential anomalies
3. Run TADE and MC.ipynb to execute the TADE algorithm and detect spatial micro-clusters


## Description


## Data
Trajectory process data of public buses provided by Stadtwerke Munich

[process model](https://github.com/qishangxin/TSMC/blob/main/Sample%20Data%20Process%20Mining%20SWM%20LSA/prozess%20modell%20(linienverlauf).csv)

The expected conduction of 

[telegram logs](https://github.com/qishangxin/TSMC/blob/main/Sample%20Data%20Process%20Mining%20SWM%20LSA/telegramme%20logs.csv)

## Modules
