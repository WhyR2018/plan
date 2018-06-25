# Correcting for SAMple BIAs with the sambia R package

[Norbert	Krautenbacher,	Institute of Computational Biology, Helmholtz Center Munich; Chair of Mathematical Modeling of Biological Systems, Technical University Munich]()

## Description

Samples taken from a population can lead to sample selection bias, for instance because of complex survey designs, and can distort statistical analyses. We introduce the R-package ‘sambia’ which is a collection of various techniques correcting statistical models for sample selection bias. We focus on correcting arbitrary classifiers for biased samples resulting from stratified random sampling.

In particular, we place the resampling-based methods ""stochastic inverse-probability oversampling"" and ""parametric inverse-probability bagging"" at the disposal which generate synthetic observations in order to resemble the original data and covariance structure. These methods have been proposed and the latter shown to outperform state-of-the-art methods for random forests in Krautenbacher, Theis, and Fuchs, “Correcting Classifiers for Sample Selection Bias in Two-Phase Case-Control Studies”, Computational and Mathematical Methods in Medicine, 2017.

