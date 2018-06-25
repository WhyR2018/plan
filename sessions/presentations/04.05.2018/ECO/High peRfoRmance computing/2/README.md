# Using the GPU for speeding up custom models in R

[Krzysztof	Jędrzejewski,	Pearson]()

## Description

Estimating values of latent model parameters is one of the most common tasks in the work of a data scientist. For most popular models, there are specialised packages that can be used for that purpose. Yet these libraries are usually limited to the most generic forms of these models, and they do not allow for much customisation. Also, they are sometimes limited by the assumptions made by their authors.

One solution for such cases is to use libraries implementing dataflow programming paradigm such as TensorFlow. They’re used most often for deep learning but they can be successfully applied to other tasks too. The added value of using such tools is the possibility to use GPU for processing, which can speed up computations up to 50 times.
I’ll talk about my journey into the world of IRT modelling. It started from using a specialised packages like TAM, but later led me to experimenting with a variety of other, more general tools. I’ll show how Tensorflow, and other tools I tried, may be used to estimate model parameters when working with datasets containing millions of observations. I’ll also compare algorithm performance results for both CPU and GPU and point out the advantages and disadvantages of using each technology.

In addition, I’ll discuss how cloud services such as AWS can be used to build a highly scalable workflow for periodical recalculations of parameters of such models, even when the total amount of data exceeds a billion observations.

