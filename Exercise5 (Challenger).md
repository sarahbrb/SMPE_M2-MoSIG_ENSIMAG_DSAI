### *1. Summary of the document "[Analysis of the risk of failure of the Challenger shuttle O-rings](https://gitlab.inria.fr/learninglab/mooc-rr/mooc-rr-ressources/blob/master/module2/exo5/challenger_fr.pdf)"*
The paper is an attempt at risk modeling based on historical data. It relies on logistic regression to estimate the probability of malfunction as a function of temperature. Although the approach is relevant, several aspects of the analysis could have been improved to provide more reliable results.

##### Positive points:
* **Methodological approach:** The use of logistic regression to model the probability of O-ring failure is appropriate, as this model allows to estimate a probability for a binary event (failure or not).

* **Pedagogical explanation:** The document includes clear explanations on the method used, in particular on logistic regression and its results. This makes the analysis understandable for readers with a background in statistics.

* **Data visualization:** The inclusion of graphs to illustrate the relationship between temperature and failure frequency allows to have a first visual idea of ​​the trend.

##### Points to improve (1st attempt):
* **Lack of data for extreme temperatures:** The analysis includes higher temperatures (above 50°F), but there is no data for temperatures as low as the launch day (31°F). Attempting to draw conclusions in an area where no data is available leads to an underestimation of the true risk.

* **Exclusion of flights without failures:** Flights where no malfunctions were recorded are excluded from the analysis, which distorts the results. Indeed, these flights provide important information on the conditions under which the seals operate correctly. Their inclusion would have allowed for a more complete analysis.

* **Uncertainty not taken into account:** The uncertainty of the estimates from the logistic regression is not sufficiently highlighted in the conclusion. The model shows a large uncertainty about the influence of temperature, but this uncertainty is not taken into account when assessing the launch risk. This gives a false impression of confidence in the results.

##### Points to improve (2nd attempt):
* **Increase sample size:** The small number of observations (23 flights in the data) limits the ability of the model to identify significant relationships. More data on flights with different temperature levels, including low temperatures such as on the day of the accident, would improve the precision of the estimates. If possible, obtaining more data, such as additional shuttle flights or additional simulations, would strengthen the conclusions.

* **Include other explanatory variables:** The current model only includes temperature as an explanatory variable. However, other factors may influence the probability of O-ring failure, such as:

    i. Pressure: Although the pressure is relatively constant in the sample (around 200 psi), it might be useful to include it to test its effect.
  
   ii. Seal age: Older seals might be more likely to fail.
  
  iii. Other environmental factors: Such as humidity or storage time before use.
  

* **Trying non-linear transformations:** The relationship between temperature and failure probability may not be linear. A significant drop in temperatures could have an exponential or quadratic effect on the failure probability.

* **Testing other statistical methods:** Logistic regression is a good model for binary probabilities, but other more robust methods might provide more reliable results, especially when the sample is small. We can test alternative methods such as:
  
    i. Ridge regression or Lasso regression : to regularize the coefficients.

   ii. Mixed effects model : to account for variations between different flights.

  iii. Bayesian analysis : to incorporate more explicit uncertainty into the model.
  

  
### *2. Notebook Updating*
* *[Initial version](https://app-learninglab.inria.fr/moocrr/jupyter/user/9f6bea3395b39c150a1a33598f831331/notebooks/work/module2/exo5/exo5_fr.ipynb)*
* The results of some tests to improve the analysis are available here : *[exo5(improved version)](https://app-learninglab.inria.fr/moocrr/jupyter/user/9f6bea3395b39c150a1a33598f831331/notebooks/work/module2/exo5/exo5(Improved%20version).ipynb)*
