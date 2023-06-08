# DREAM_PACKAGE: Bayesian inference using MCMC simulation with the DREAM/DREAM_D/DREAM_ZS/DREAM_DZS algorithms

## Description

Bayesian inference has found widespread application and use in science and engineering to reconcile Earth system models with data, including prediction in space (interpolation), prediction in time (forecasting), assimilation of observations and deterministic/stochastic model output, and inference of the model parameters. Bayes theorem states that the posterior probability, $p(H|\tilde{\textbf{Y}})$ of a hypothesis, $H$ is proportional to the product of the prior probability, $p(H)$ of this hypothesis and the likelihood, $L(H|\tilde{\textbf{Y}})$ of the same hypothesis given the new observations, $\tilde{\textbf{Y}}$, or $p(H|\tilde{\textbf{Y}}) \propto p(H) L(H|\tilde{\textbf{Y}})$. In science and engineering, $H$ often constitutes some numerical model, $\mathcal{F}(\textbf{x},\cdot)$ which summarizes, in algebraic and differential equations, state variables and fluxes, all knowledge of the system of interest, and the unknown parameter values, \textbf{x} are subject to inference using the data $\tilde{\textbf{Y}}$. Unfortunately, for complex system models the posterior distribution is often high dimensional and analytically intractable, and sampling methods are required to approximate the target. In the attached paper I review the basic theory of Markov chain Monte Carlo (MCMC) simulation and introduce a MATLAB toolbox of the DiffeRential Evolution Adaptive Metropolis (DREAM) algorithm developed by \cite{vrugt2008a,vrugt2009a} and used for Bayesian inference in fields ranging from physics, chemistry and engineering, to ecology, hydrology, and geophysics. This MATLAB toolbox provides scientists and engineers with an arsenal of options and utilities to solve posterior sampling problems involving (among others) bimodality, high-dimensionality, summary statistics, bounded parameter spaces, dynamic simulation models, formal/informal likelihood functions (GLUE), diagnostic model evaluation, data assimilation, Bayesian model averaging, distributed computation, and informative/noninformative prior distributions. The DREAM toolbox supports parallel computing and includes tools for convergence analysis of the sampled chain trajectories and post-processing of the results. Seven different case studies illustrate the main capabilities and functionalities of the MATLAB toolbox.

## Getting Started

### Installing

* Download and unzip the zip file 'MATLAB_pcode_DREAM_PACKAGE_V2.0.zip'.
* Add the toolbox to your MATLAB search path by running the script 'install_DREAM_PACKAGE.m' available in 'MATLAB_pcode_DREAM_PACKAGE_V2.0'
* You are ready to run the examples.

### Executing program

* After intalling, you can simply direct to each example folder and execute the local 'example_X.m' file.
* Please make sure you read carefully the instructions (i.e., green comments) in 'install_DREAM_PACKAGE.m' and the manual in PDF !!!  
* Please also refer to the Addendum PDF which describes the changes made to integrate DREAM/DREAM_D/DREAM_ZS/DREAM_DZS algorithms into one toolbox/

## Authors

* Vrugt, Jasper A. (jasper@uci.edu) 

## Version History

* 1.0
    * Initial Release
* 2.0 
    * Merged DREAM/DREAM_ZS/DREAM_D/DREAM_DZS and DREAM_BMA into one algorithm.
    * Latest update to case study 6 to show how to work with generalized/universal likelihood functions described in the paper: 
         Vrugt, J.A., D.Y. de Oliveira, G. Schoups, and C.G.H. Diks (2022), On the use of distribution-adaptive likelihood functions: Generalized and universal likelihood functions, scoring rules and multi-criteria       
         ranking, Journal of Hydrology, 615, Part B, 2022, doi:10.1016/j.jhydrol.2022.128542: https://www.sciencedirect.com/science/article/pii/S002216942201112X

## Acknowledgments
