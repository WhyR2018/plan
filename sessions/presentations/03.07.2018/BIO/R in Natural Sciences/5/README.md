# PCRedux: machine learning helper tool for sigmoid curves

[Stefan	Rödiger,	BTU Cottbus - Senftenberg]()

## Description

There are numerous examples of data with a sigmoid ('S'-shaped) curves in data science. One example is amplification curve data from quantitative Polymerase chain reactions (qPCR). The qPCR is an indispensable technology in human diagnostics and forensics. From an amplification curve quantitative information can be determined which can be used to assess diseases.

There are software packages, which offer workflows and criteria to process the qPCR data. That includes the preprocessing of the raw data, the fitting of non-linear models on raw data, the calculation of quantification points, the computation of amplification efficiency, the relative gene expression analysis, normalization procedures and data management. However, there is no open source software package that contains classified data sets and provides biostatistical methods for machine learning on amplification curves. 

The `PCRedux` package contains functions and classified amplification curves for machine learning and statistical analysis. In addition, the PCRedux package contains extensive labelled data sets of amplification curves from various qPCR devices and detection chemistries. The amplification curves were classified (negative, positive) by a human. For curve shape based classification, the `tReem()` funftion was developed. To analyze the amplification curves methods such as change-point analysis, regression analysis, autocorrelation analysis and model fitting have been integrated. The `pcrfit_single()` function calculate more than 45 features from the amplification curves. This is useful for creating models and predicting classes (e. g. negative, positive). 

Additional functionality in the package includes:
- `decision_modus()`, which calculates the frequency of classes in a data set,
- `earlyreg()`, which calculates features by a regression analysis in the background region,
- `head2tailratio()`, which compares the ratio of the head and tail,
- `hookregNL()` and `hookreg()`, which attempt to detect a hook effect in the amplification curve,
- `mblrr()`, which performs local robust regressions analysis,
- `performeR()`, which performance analysis (e.g., sensitivity, specificity, Cohen's kappa) for binary classification and
- `encu()`, which enables high-throughput data processing.

A prototype of the PCRedux web server for the analysis of amplification curves using the PCRedux package is available from http://www.smorfland.uni.wroc.pl/shiny/predPCR/. The web server uses the machine learning `mlr` package as interface to a large number of classification and regression techniques. The `PCRedux` can be used for the extraction of features and for machine learning on amplification curves. The `PCRedux` package is an add-on package (MIT license) for open source statistical computing language and environment R.