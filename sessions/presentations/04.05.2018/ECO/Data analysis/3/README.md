# auditor: an R package and methodology for validation of any statistical model

[Alicja	Gosiewska,	MI2 DataLab, Warsaw University of Technology]()

## Description

Predictive modeling is the branch of statistics concerned with finding a model that best reflects the data-generating process. Lots of machine learning algorithms in this area have been developed and is still developing, therefore there are countless possible options to choose from and a lot of ways to do it. Predictions of a poorly fitted model will be misleading when confronted with future data, which is unacceptable and potentially hazardous in many cases, for example in medicine.  That is why methods that support the selection of proper model are important.

During this talk, I will introduce the auditor package which is a uniform interface to statistics and  visualizations that facilitate assessing and comparing the goodness of fit, performance, diagnostic and similarity of models.  As it concentrates on the analysis of residuals, most of the presented methods are model-agnostic. In this talk I will present examples for classification and regression models.
Moreover, the auditor is designed to make validation more convenient and accessible by reducing the amount of effort needed to create informative visualizations, for both commonly used plots and new approaches.

References:
-  Alicja Gosiewska and Przemyslaw Biecek (2018). auditor: Model Audit - Verification, Validation, and Error Analysis. R package version 0.2.1. [https://mi2-warsaw.github.io/auditor/]
- Yuan Tang, Masaaki Horikoshi, and Wenxuan Li. ""ggfortify: Unified Interface to Visualize Statistical Result of Popular R Packages."" The R Journal 8.2 (2016): 478-489.
- Przemyslaw Biecek (2018). DALEX: Descriptive mAchine Learning EXplanations. R package version 0.2.0. [https://CRAN.R-project.org/package=DALEX]

