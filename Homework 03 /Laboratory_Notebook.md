# Laboratory Notebook "user pointing experiment"

###### *Empirical evaluation of [Fitts’s law](https://en.wikipedia.org/wiki/Fitts%27s_law): Fork this small [project](https://gricad-gitlab.univ-grenoble-alpes.fr/coutrixc/m2r_pointingxp)*

## General organization

#### *data/*
This folder contains both raw and processed experimental data that is returned from the experimental software.
Each file name is named after the following format: "*DD-MM-YYYY_xxx*" where 'xxx' is either:
- RawData : the raw data  as returned from the experimental software.
- MeanMTData : the processed mean movement times as returned from the experimental software.

#### *analysis/*
This folder contains my R markdown script used to analyze the data collected from the experiment.

## Experimental Reports


#### *Experimental task*
I used the implementation of a [pointing experiment from Ergonomics Web at Cornell University](https://ergo.human.cornell.edu/FittsLaw/FittsLaw.html). On this Webpage, one can gather data for controlled 1D user pointing experiments.

#### *Experimental variables* 
I ran the experiment from the above Webpage with 1, 2 and 4 widths and with 16, 32 and 64 distances, with 6 trials for each combination (Same as Teacher).

#### *Data collected*
The Webpage returned the following [results](https://github.com/sarahbrb/SMPE_M2-MoSIG_ENSIMAG_DSAI/blob/main/Homework%2003%20/data%20/Fitts'%20Law%20Experiment%20(Results).pdf):

* I performed 26 pointing errors
* A Fitts modeling in the form of MT = 511.627 + 144.326log(A/W + 1) with R² = 0.478
* The table of mean MT that I provide in the [data folder](https://github.com/sarahbrb/SMPE_M2-MoSIG_ENSIMAG_DSAI/tree/main/Homework%2003%20/data%20).
* The table of raw pointing data that I provide in [data folder](https://github.com/sarahbrb/SMPE_M2-MoSIG_ENSIMAG_DSAI/tree/main/Homework%2003%20/data%20). 



#### *Data analysis*
My data analysis performed and commented is available here : [user pointing experiment analysis](https://github.com/sarahbrb/SMPE_M2-MoSIG_ENSIMAG_DSAI/blob/main/user_pointing_experiment_analysis.ipynb).
