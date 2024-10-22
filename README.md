# Homework 1st Week : 26/09/2024

- [x] Indicate your name on the [PAD](https://codimd.math.cnrs.fr/s/GYhTSQxFu#Welcome-to-the-SMPE-2024-2025-pad).
- [x] Register on the Mattermost : @sarahbrb
- [x] Set up a public github repository for this lecture : https://github.com/sarahbrb/SMPE_M2-MoSIG_ENSIMAG_DSAI
- [x] Register to the MOOC.
- [x] Follow modules 1 + 2 of the MOOC with as much exercises as possible.
- [x] Set up a computational document system (e.g., Rstudio or Jupyter) on your laptop.
- [x] Report the URL of your git project, your mattermost ID on the [PAD](https://codimd.math.cnrs.fr/s/GYhTSQxFu#Welcome-to-the-SMPE-2024-2025-pad).
- [x] Start learning R by reading my short R crash course for computer scientists.

# Homework 2nd Week : 03/10/2024

- [x] Read Popper’s text and write a short summary in your GitHub repository

#### *Summary of Karl Popper's Conjectures and Refutations*
In Conjectures and Refutations, Karl Popper explores the difference between science and pseudo-science. He argues that the key feature of a scientific theory is its falsifiability, the ability to be tested and potentially proven wrong by evidence. While pseudo-scientific theories (like astrology, Freudian psychology, or Marxism) explain everything and cannot be refuted, true scientific theories make bold predictions that can be tested and, if found false, rejected. Popper emphasizes that genuine scientific progress is made by proposing theories that risk refutation and undergoing rigorous testing. He concludes that falsifiability is the criterion that separates scientific knowledge from non-scientific beliefs.

- [ ] Criticize every figure of Jean-Marc’s slides by:
 * i. Applying the checklist for good graphics;
 * ii. Proposing a better representation (hand-drawing is fine) that passes the checklist.

"Une brève histoire de l'informatique" Figure:
| Critics            | Proposed Improvements           |
| -------------      | -------------                  |
| The text is somewhat small and cramped, making it hard to read, especially for smaller elements like technical names.       | Create a clearer, multi-tier timeline separating science, technology, and social impacts.                              |
| The use of different colored areas is useful to show societal impact and technological advances, but the yellow area could be more distinct from other parts.                | Increase the font size for important events, and reduce the density of less critical information.                             |
| The overlapping of the colored regions makes it hard to interpret which elements belong to which category. For example, the boundaries between the "Applications" and "Impact sociétal" categories are not clear.            | Use cleaner color blocks with better contrast to differentiate different aspects (e.g., science, technology) without overlapping, and add legends for clarity.                |
| There is a lot of data crammed into the image, making it overwhelming and less accessible. The differentiation between historical periods is hard to grasp quickly. | Use symbols or icons for key innovations, such as the invention of the Internet or the appearance of PCs, to make it easier to quickly understand. |
|The title and major events (e.g., the appearance of FORTRAN, Internet, etc.) are not emphasized enough compared to less significant events.| |


- [ ] Report this work for at least 3 figures on you github/gitlab project.
- [x] MOOC: Complete exercise 5 of module 2 (Challenger). Write a short text explaining what is good and wrong about this document (you may want to provide an updated version of the notebook) and upload on your github/gitlab space.

#### *1. Summary of the document "Analysis of the risk of failure of the Challenger shuttle O-rings"*
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
  

  
#### *2. Notebook (Improved version) :*
The results of some tests to improve the analysis are available here : *[exo5(improved version)](https://app-learninglab.inria.fr/moocrr/jupyter/user/9f6bea3395b39c150a1a33598f831331/notebooks/work/module2/exo5/exo5(Improved%20version).ipynb)*
  
 # Homework 4th Week : 17/10/2024
- [ ] Continue the hands-on, improve the experiment design and the analysis



 
