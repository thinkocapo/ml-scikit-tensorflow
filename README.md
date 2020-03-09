# ml

virtualenv -p /usr/bin/python3 ml_env

## Setup
$ python3 -m ipykpip install -U jupyter matplotlib numpy pandas scipy scikit-learn
$ python3 -m ipykernel install --user --name=python3
$ python3 -m ipykernel install --user --name=python3
Installed kernelspec python3 in /home/wcap/.local/share/jupyter/kernels/python3

## Run
jupyter notebook

## Data
https://github.com/ageron/handson-ml2

## Questions

Housing - Supervised Learning + Regression
"predict a district's median housing price, given other data baout that district"
p52
random generator seed + hash
"set the random number gneerator's seed before calling random.permutation, so that it always generates the same shuffled indices.
But this will break the next time you fetch an updated dataset.
"compute a cash of each instance's identifier and put thati nstance in the test set if the hash is lower than or eqaul to 20% of the maximum hash value.
"this insures that the test set willremain consistent across multiple runs, even if you refresh the dataset"

p53 
^ no good unique identifier yet, so compute one based on stable features
"use the row index as a unique identifier, you need to make sure that new data gets appended to the end of the dataset and that no row ever gets deleted.

p55 stratified vs purely random sampling
split.split?