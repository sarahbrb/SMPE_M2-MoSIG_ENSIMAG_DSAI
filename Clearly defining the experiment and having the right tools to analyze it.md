# Laboratory Notebook for a user pointing experiment

###### *Empirical evaluation of [Fitts’s law](https://en.wikipedia.org/wiki/Fitts%27s_law): Fork this small [project](https://gricad-gitlab.univ-grenoble-alpes.fr/coutrixc/m2r_pointingxp)*

## General organization

#### *data/*
This folder contains both raw and processed experimental data that is returned from the experimental software.
Each file name is named after the following format: "*3rd session SMPE Project - data*" where 'data' is either:
- Raw Data : the raw data  as returned from the experimental software.
- Table of Mean MT : the processed mean movement times as returned from the experimental software.

#### *analysis/*
This folder contains my R markdown script used to analyze the data collected from the experiment.

## Experimental Reports

#### *Experimental task*
I used the implementation of a [pointing experiment from Ergonomics Web at Cornell University](https://ergo.human.cornell.edu/FittsLaw/FittsLaw.html). On this Webpage, one can gather data for controlled 1D user pointing experiments.

#### *Experimental variables* 
I ran the experiment from the above Webpage with 1, 2 and 4 widths and with 16, 32 and 64 distances, with 6 trials for each combination. (Same as Teacher).

#### *Data collected*
The Webpage returned the following results:

* I performed 26 pointing errors
* A Fitts modeling in the form of MT = 511.627 + 144.326log(A/W + 1) with R² = 0.478
* The table of mean MT that I provide in the data folder : 
* The table of raw pointing data that I provide in data folder : 


#### *Data analysis*
My data analysis is performed and commented in the [xxx]() file.
