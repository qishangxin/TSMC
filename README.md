# TSMC - Temporal and Spatial Micro-Clustering
Temporal and spatial micro-clustering of trajectory process data, based on the method of TADE - Temporal Activity Density Estimation.

# Table of Contents
* [Setup](#setup)
* [Use Instructions](#use-instructions)
* [Description](#description)
* [Data](*data)
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
This project aims at experimenting the noval [TADE](https://link.springer.com/chapter/10.1007/978-3-030-58666-9_13) algorithm, Temporal Activity Density Estimation, in a real world case. We implement the algorithm and test different configurations on the trajectory process data of certain public bus lines of Munich. We detect three types of anomalies among the data and find out micro-clusters containing high percentage of anomaly based on the time interval anomalies. The evaluation results show that the most evident micro-clusters are indeed where heavy delay takes place.


## Data
Trajectory process data of public buses provided by Stadtwerke Munich.

[process model](https://github.com/qishangxin/TSMC/blob/main/Sample%20Data%20Process%20Mining%20SWM%20LSA/prozess%20modell%20(linienverlauf).csv)

The expected conduction of provided bus lines.

[telegram logs](https://github.com/qishangxin/TSMC/blob/main/Sample%20Data%20Process%20Mining%20SWM%20LSA/telegramme%20logs.csv)

## Modules
The project owns the following python modules:

* [pre-TADE](#pre-TADE)
* [TADE and MC](#TADE-and-MC)

### pre-TADE
Pre-processing of the data logs mentioned above. It also serves to find out the numerical and sequential anomalies from the data.

### TADE and MC
Implementation of the TADE algorithm, the formation of micro-clusters as well as the visualization of the final results.


## Others
[merged_log](https://github.com/qishangxin/TSMC/blob/main/notebooks/merged_log.csv) is a merged log with all the necessary information after data cleaning for the later implementation of TADE and MC.

[(Back to top)](#table-of-contents)
