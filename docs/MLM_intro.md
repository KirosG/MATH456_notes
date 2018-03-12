
# (PART) Multi-level Modeling {-}


# Introduction

The assumption of independence between observations is often violated $Cor(\epsilon_i, \epsilon_j)\neq 0, \forall i\neq j$

* Sampling students within schools. (Within school correlation)
* Repeatedely measuring the same tree in different places. (Within-subject correlation)
* Repeatedly measuring the same tree over time. (Temporal correlation)
* Poverty measurements from different, but neighboring, counties. (Spatial correlation)

When data are _clustered_, we need to adjust how we model the structure of the error terms to account for this correlation. 


This section of the notebook is organized as follows: 

1. We introduce the concept of clustering and intraclass-correlation via random effects ANOVA. 
2. We then introduce the concept of pooling and expand this model to include other covariates by fitting a Random Intercept model
3. We then discuss and demonstrate two specialized types of clustered data
    - Longitudinal (Time series) measurements - correlated in time 
    - Geographic measurments - correlated in space