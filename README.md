# A Probabilistic Framework for Evaluating Football Player Performance on a Global Scale

This repository contains an example of how the proposed methodology in [journal paper link here] is used in practice.

## Methodology Summary

The methodology consists of couple of main steps:

1. Creation of scaling coefficients to incorporate contextual factors
2. Scaling of the raw in-game player statistics
3. Aggregation of raw statistics to represent overall performance of the player. This aggregation is done in three main ways: Regular averages, ratios of scaled statistics and a so-called "strength" variable that measures the success ratio as well as the effect size
4. Ranking of aggregated features using Empirical Cumulative Distribution estimation
5. Weighted geometric average of aggregated feature rankings to arrive at a single player rating

## Data

"This repository uses the publicly available Events dataset by WyScout to perform calculations."[[1]](#1)

The dataset can be found [here](https://www.nature.com/articles/s41597-019-0247-7)

## Code

This repository contains minimally reproducible

## References
<a id="1">[1]</a> 
Pappalardo, L., Cintia, P., Rossi, A. et al. 
A public data set of spatio-temporal match events in soccer competitions. 
Sci Data 6, 236 (2019). 
https://doi.org/10.1038/s41597-019-0247-7