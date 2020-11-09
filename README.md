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

This repository uses the publicly available Events dataset by WyScout [[1]](#1) to perform calculations.

The dataset can be found [here](https://www.nature.com/articles/s41597-019-0247-7).

## Code

This repository contains minimally reproducible code for R and Python to access public API for making computations. While the sample code is provided in R and Python, REST API can be accessed through any programming language who can perform HTTP requests to a server. The API request takes in user configurations and outputs the following data based on those:

1. User & Scale configuration object
2. Raw in-game statistics that fit the criteria. For instance, if the date window is selected between '2017-08-30' and '2018-01-01', only the data for this period will be returned.
3. Computed scale coefficients for the matches that fit the criteria
4. Per 90 scaled averages of player statistics
5. Features computed through the methodology
6. Player rankings object

Global Soccer Rankings Public API documentation can be viewed [here](http://globalrankings.io/redoc), for details on query parameters and outputs.

<!-- Add the link to feature descriptions -->
The details of feature descriptions are provided [here](https://github.com/Aelvangunduz/globalplayerrankings/blob/main/docs/feature_descriptions.md). 

The raw statistics definitions can be obtained from [WyScout API Docs](https://apidocs.wyscout.com/#tag/Advanced-Stats/paths/~1players~1{wyId}~1matches~1{matchWyId}~1advancedstats/get).

## References
<a id="1">[1]</a> 
Pappalardo, L., Cintia, P., Rossi, A. et al. 
A public data set of spatio-temporal match events in soccer competitions. 
Sci Data 6, 236 (2019). 
https://doi.org/10.1038/s41597-019-0247-7