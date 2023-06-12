# An Analytical Effective Point-Source-Based Distance-Conversion Approach to Mimic the Effects of Extended Faults on Seismic Hazard Assessment

## Table of Contents

+ [Overview](#overview)
+ [Abstract](#abstract)
+ [Citation](#citation)

## Overview
The main function to estimate the effective hypocentral and epicentral distances is as follows:

[Reff_hyp_theta,Reff_epi_theta] = DIST_CONVERT(r_jb,dip,L,W,Ztor,theta,grid_strike,grid_width,Vs,freq);

The input parameters that are required to define or assign by the user are Joyner–Boore (JB) distance, dip angle, fault length, fault width, depth to the top of rupture, azimuth angle, number of cells along the strike, number of cells along the width, shear-wave velocity, and frequency of interest, respectively.

There are two other functions to account for the effects of geometric spreading and quality factor functions. They can be updated by the user regarding the seismological characteristics of the area of interest. There are also two examples to clarify how to use the code. Note that DIST_CONVERT is a pcode and cannot be opened and modified.

## Abstract <a name = "abstract"></a>
Data-driven ground motion models (GMMs) for the average horizontal component from shallow crustal continental earthquakes in active tectonic regions are derived using a subset of the NGA-West2 dataset including 14518 recordings out of 285 earthquakes recorded at 2347 different stations. We use four different nonparametric supervised machine learning (ML) algorithms including Artificial Neural Network, Kernel-Ridge Regressor, Random Forest Regressor, and Support Vector Regressor to construct four individual models. Then, we use a weighted average ensemble approach to combine these four models into a robust model to predict various ground motion intensity measures such as peak ground displacement (PGD), peak ground velocity (PGV), peak ground acceleration (PGA), and 5%-damped pseudo-spectral acceleration (PSA). The model input parameters are moment magnitude, rupture distance, VS30, and ZTOR. The ensemble modeling attempts to remove the drawbacks or deficiencies of different ML algorithms while capturing their advantages and also accounts for epistemic uncertainty. Although no functional form is provided, the model is able to capture salient features observed in ground motions such as saturation as well as geometrical spreading, anelastic attenuation, and nonlinear site amplification. The response spectra, as well as the magnitude, distance, VS30, and ZTOR scaling trends, are consistent and comparable with the NGA-West2 GMMs including several additional input parameters. We used a mixed-effects regression analysis to split the total aleatory uncertainty into between-event, within-station, and event-site-corrected components. The model is applicable to magnitudes from 3.0 to 8.0, rupture distances up to 300 km, and spectral periods of 0 to 10 s. 


## Citation <a name = "citation"></a>
Tavakoli, B., Sedaghati, F., & Pezeshk, S. (2018). An Analytical Effective Point‐Source‐Based Distance‐Conversion Approach to Mimic the Effects of Extended Faults on Seismic Hazard AssessmentAnalytical Effective Point‐Source‐Based Distance‐Conversion Approach. Bulletin of the Seismological Society of America, 108(2), 742-760. https://doi.org/10.1785/0120170171
