# Application of mlr and ggplot for machine-learning and visualisation on multiple depended variables

[Jaroslaw	Jasiewicz,	Adam Mickiewicz University]()

## Description

We want to present application of mlr package and ggplot grammar of graphics to build a complete learning and presentation system addressed for soil science. Modeling of soils properties based on the satellite images is a leading task in modern remote sensing. While modeling of a single attribute is rather straight-forward process proper modeling of multiple features using multiple learners and several data transformations leads to the combinatorial explosion of possible variants of solutions. Also, prediction of different soil properties gain its highest performance with different learners and sets of model hiper-parameters so searching for the optimal solution for each parameter may be a tedious and time-consuming process but, first of all, difficult to preset due to multidimensional nature of the results.

Our data set includes 150 points sampled in the area near Pokrzywno (Poznań) from two separate field crops. Sixteen chemical properties of soils (nutrients) determined in the wet laboratory. An eight spectral channels data acquired from WorldView-2 repository was used to build machine learning regression models between nutrients and radiometric response of soil surface. We used several popular learners (glm, r-Forest, Qubist, k-SVM, kKNN, PLS-R MARS and CR-splines). Input data were used as a raw data, transformed by contrast-stretch and Box-Cox universal transformation. 

There are three problems in our research: 
- how to treat data collected from two similar, yer separate sources
- how a transformation of the data affects the performance of different learners
- which learner is performing best on each nutrient? We noticed that different nutrients gain the best prediction for different learners and the difference is significant.

Such approach raises several problems at the level of data processing and processing:
- how to run multiple learning/prediction/performance analysis processes in a single routine
- how to present such four-dimensional (learner-transformation-nutrient-crop field) results in a clear and human readable form?

To solved that problems applied mlr package due to universality, transparent proceeding, and easiness of batch processing, then the results were transformed with dplyr and we prepared set of ggplot routines to clearly visualize four-dimensional results in a form of single 2D plot. The simple analysis of the plot indicates best learners for given nutrient as well shows which method of transformation minimizes the impact of sampling on various arable fields (Box-Cox transformation)